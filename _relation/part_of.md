---
layout: entry
title: "part_of"
shortdef: "Relationships between whole and part"
order: 4
---

This relation indicates the relationships between whole entity and its part.  

Typical examples are relationships between [Cell]() and its [Anatomical_entity](), or [Cell_component]() and [Cell]().

~~~ ann
Mitochondria in lung epithelial cells.
T1 Cell_component 0 12 Mitochondria
T2 Cell 21 37 epithelial cells
T3 Anatomical_entity 16 20 lung
R1 part_of Arg1:T1 Arg2:T2
R2 part_of Arg1:T2 Arg2:T3
~~~
~~~ ann
lung alveolar epithelial cell migration
T1 Anatomical_entity 0 4 lung
T2 Cell 5 29 alveolar epithelial cell
T3 Localization 25 39 cell migration
E1 Localization:T3 Theme:T2 AtLoc:T1
R1 part_of Arg1:T2 Arg2:T1
~~~

<!---
Typical examples are [Cell]() and its [Cell_component](), or [Protein_molecule]() and [Amino_acid_monomer]().


{% include image.html name="whole-part-example.png" width="70%" %}


~~~ ann
Ser200 acts as a nucleophile at the active site of AChE.
T1 Amino_acid_monomer 0 6 Ser200
T2 Protein_molecule 51 55 AChE
R1 part_of Arg1:T1 Arg2:T2
~~~
--->
