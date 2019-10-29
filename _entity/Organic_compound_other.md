---
layout: entry
title: "Organic_compound_other"
shortdef: "Organic Compound, excluding medicine (GENIA)"
order: 20
---

The name of this entity group is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This entity is based on <a href="https://www.ebi.ac.uk/chembl/">ChEMBL</a> database.

Organic compounds, such as metabolites, are categorized into this entity group.

The following molecules can be categorized into this entity group.
- carbohydrates
- nucleotides
- lipid molecules

The definition of 'Organic_compound_other' (Organic compounds/metabolites) is based on the Semantic types of
- 'orch' (Organic Chemical)
- 'carb' (Carbohydrate)
- 'eico' (Eicosanoid)
- 'lipd' (Lipid)
- 'strd' (Steroid)
- 'vita' (Vitamin)
- 'horm' (Hormone) (if it is not composed of peptides/proteins)
- 'nnon' (Nucleic Acid, Nucleoside, or Nucleotide) (if it is metabolite instead of part(s) of genes/gene prodcuts)
- 'bacs' (Biologically Active Substance) (if it is not peptides/proteins)

in the <a href="https://www.nlm.nih.gov/research/umls/">UMLS database</a>.

~~~ ann
The alpha-phosphate of ATP.
T1 Organic_compound_other 23 26 ATP
~~~
~~~ann
T cell blasts were treated with PMA.
T1 Cell 0 13 T cell blasts
T2 Artificial_process 19 26 treated
T3 Organic_compound_other 32 35 PMA
E1 Artificial_process:T2 Theme:T1 Theme2:T3
~~~

<!-- details -->
