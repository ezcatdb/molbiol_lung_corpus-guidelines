---
layout: entry
title: "Cell"
shortdef: "Cell types and cell lines"
order: 11
---

This entity group is based on Cell_natural and Cell_cultured in the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This entity is based on 
<a href="https://www.ebi.ac.uk/ols/ontologies/cl">
Cell ontlogy
</a> or 
<a href="https://www.ebi.ac.uk/ols/ontologies/clo">
Cell line ontology
</a>.

'Cells' are categorized into this entity group.

The following words/phrases are examples of this entity.

- epithelial cells (UMLS ID:C0014597)
  - alveolar epithelial cells (UMLS ID:C0225698)
- endothelial cells
  - capillary endothelial cells
- fibroblasts (UMLS ID:C0016030)

- platelets (= thrombocytes)（血小板）
- white blood cells (= leukocytes)（白血球）
  - monocytes (= mononuclear phagocytes)（単球）
    - macrophages (= phagocytes)
    - dendritic cells (樹状細胞)
    - osteoclasts (破骨細胞)
  - lymphocytes（リンパ球）
    - T lymphocytes (= T cells)
      - T lymphoblasts (= T cell blasts)
  - granulocytes (= polymorphonuclear leucocytes = blood granulocytic cells = granular leukocytes)(顆粒球)
    - neutrophils (= neutrophiles)（好中球）
    - eosinophil granulocytes　（好酸球）
    - basophils (好塩基球)


~~~ ann
Cellular crosstalk between epithelial cells and fibroblasts.
T1 Cellular_process 0 18 Cellular crosstalk
T2 Cell 27 43 epithelial cells
T3 Cell 48 59 fibroblasts
E1 Cellular_process:T1 Participant:T2 Participant2:T3
~~~
~~~ann
T cell blasts were treated with PMA.
T1 Cell 0 13 T cell blasts
T2 Artificial_process 19 26 treated
T3 Organic_compound_other 32 35 PMA
E1 Artificial_process:T2 Theme:T1 Theme2:T3
~~~
~~~ ann
lung alveolar epithelial cell migration
T1 Anatomical_entity 0 4 lung
T2 Cell 5 29 alveolar epithelial cell
T3 Localization 30 39 migration
E1 Localization:T3 Theme:T2 AtLoc:T1
R1 part_of Arg1:T2 Arg2:T1
~~~

The following cases are complicated:
~~~ ann
human lung fibroblasts (HLFs)
T1 Subject 0 5 human
T2 Anatomical_entity 6 10 lung
T3 Cell 11 22 fibroblasts
T4 Cell 0 22 human lung fibroblasts
T5 Cell 24 28 HLFs
R1 part_of Arg1:T3 Arg2:T2
R2 part_of Arg1:T2 Arg2:T1
R3 member_of Arg1:T4 Arg2:T3
R4 is_equivalent Arg1:T5 Arg2:T4
~~~
~~~ ann
pulmonary fibroblast (PF)
T1 Anatomical_entity 0 9 pulmonary
T2 Cell 10 20 fibroblast
T3 Cell 0 20 pulmonary fibroblast
T4 Cell 22 24 PF
R1 part_of Arg1:T2 Arg2:T1
R2 member_of Arg1:T3 Arg2:T2
R4 is_equivalent Arg1:T4 Arg2:T3
~~~

<!-- details -->
