---
layout: entry
title: "Cell_component"
shortdef: "Cellular components, including organelle (GENIA)"
order: 12
---

The name of this entity group is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

<!--
This entity is based on 
<a href="https://www.ebi.ac.uk/ols/ontologies/cl">Cell ontology</a> 
and cellular component
(<a href="http://amigo.geneontology.org/amigo/term/GO:0005575">GO:0005575</a>) from 
<a href="http://geneontology.org/">Gene ontology</a>.
-->

The definition of ‘Cell component’ is based on the Semantic types of
-    ‘celc’ (Cell Component)

in the <a href="https://www.nlm.nih.gov/research/umls/">UMLS database</a>.

'Cell component' is categorized into this entity group.

The following words/phrases are examples of this entity.
- cytoplasm
- cytosol
- nucleus (UMLS ID:C0007610)
  - nuclear (UMLS ID:C0007610)
- transmembrane
- plasma membrane
- extracellular matrix
- mitochondria

~~~ ann
Accumulation of damaged mitochondria in lung epithelial cells.
T1 Localization 0 12 Accumulation
T2 Negative_regulation 16 23 damaged
T3 Cell_component 24 36 mitochondria
T4 Cell 40 61 lung epithelial cells
T5 Anatomical_entity 40 44 lung
E1 Localization:T1 Theme:T3 AtLoc:T4
E2 Negative_regulation:T2 Theme:T3
R1 part_of Arg1:T3 Arg2:T4
R2 part_of Arg1:T4 Arg2:T5
~~~


<!-- details -->
