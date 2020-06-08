---
layout: entry
title: "Inorganic_compound"
shortdef: "Inorganic compound, including metal ions (GENIA)"
order: 19
---

<!---
{% include image.html name="cofactors.png" width="60%" %}
--->

The name of this entity group is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This entity is based on <a href="https://www.ebi.ac.uk/chembl/">ChEMBL</a> database.

Inorganic compounds are typically chemicals which do not contain "carbon-hydrogen" bonds.
This entity usually contains metal ions.

~~~ ann
The required divalent metal ion cofactor for EcoRV
T1 Inorganic_compound 13 31 divalent metal ion
T2 Protein_molecule 45 50 EcoRV
~~~

~~~ ann
Mg2+ ion as a cofactor
T1 Inorganic_compound 0 8 Mg2+ ion
~~~

~~~ ann
Phospho-S6
T1 Conversion 0 7 Phospho
T2 GGPs 8 10 S6
T3 GGPs 0 10 Phospho-S6
T4 Inorganic_compound 0 7 Phospho
E1 Conversion:T1 Theme:T2 Product:T3
R1 part_of Arg1:T4 Arg2:T3
~~~


<!-- details -->
