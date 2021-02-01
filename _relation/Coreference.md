---
layout: entry
title: "coreference"
shortdef: "Co-referent relation; from common expression to more specific/concrete expression (mainly anaphora)"
order: 10
---
The relation, 'coreference', is used when additional expressions refer to the same thing, which is usually located prior to the expressions (anaphora). 
This relation connects common expression to more specific/concrete expression.

There are two types of coreference, entity coreference and event coreference.
However, for this corpus, only entity coreference is annotated.

The following case is an example of entity coreference.
~~~ ann
CD73, the enzyme protein which produces adenosine.
T1 GGPs 0 4 CD73
T2 GGPs 10 24 enzyme protein
T3 Organic_compound_other 40 49 adenosine
T4 Molecular_function 31 39 produces
E1 Molecular_function:T4 Theme:T3 Cause:T2
R1 Coreference Arg1:T2 Arg2:T1
~~~

