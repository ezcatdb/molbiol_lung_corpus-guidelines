---
layout: entry
title: "GGPs"
shortdef: "Gene or gene products (GENIA)"
order: 31
---

The name of this entity group, 'Gene or gene products' is based on the Protein/RNA/DNA from <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

<!--
This entity is based on 
<a href="https://www.uniprot.org/">UniProt</a> database and <a href="https://pir.georgetown.edu/pro/"> PIR ontology</a>.
-->

The definition of 'GGPs' (Gene or Gene products) is based on the Semantic types of 
- 'aapp' (Amino Acid, Peptide, or Protein), 
- 'enzy' (Enzyme),
- 'rcpt' (Receptor), 
- 'horm' (Hormone) (if it is composed of peptides/proteins),
- 'gngm' (Gene or Genome),
- 'nnon' (Nucleic Acid, Nucleoside, or Nucleotide) (if it is part(s) of genes/gene prodcuts)

in the <a href="https://www.nlm.nih.gov/research/umls/">UMLS database</a>.

However, some data of UMLS 'horm' might be for [Organic_compound_other]().

Some data of UMLS 'nnon' also may be for [Organic_compound_other](), if they are metabolites, instead of parts of genes/gene products.

Protein molecules, gene products, and genes are categorized into this entity group.
- interleukin (UMLS ID:C0021764)
- IL (UMLS ID:C0021764)
- PINK1 gene (UMLS ID:C1422771)

~~~ ann
Patients with high MMP-9 levels.
T1 Subject 0 8 Patients
T2 GGPs 19 24 MMP-9
~~~

~~~ ann
matrix metalloproteinase 9 (MMP-9), myeloperoxidase (MPO), and arginase 1 (ARG1)
T1 GGPs 0 26 matrix metalloproteinase 9
T2 GGPs 28 33 MMP-9
T3 GGPs 36 51 myeloperoxidase
T4 GGPs 53 56 MPO
T5 GGPs 63 73 arginase 1
T6 GGPs 75 79 ARG1
R1 is_equivalent Arg1:T2 Arg2:T1
R2 is_equivalent Arg1:T4 Arg2:T3
R3 is_equivalent Arg1:T6 Arg2:T5
~~~
~~~ ann
VEGFR-TKI
T1 GGPs 0 5 VEGFR
T2 Pharmacological_substance 6 9 TKI
T3 Pharmacological_substance 0 9 VEGFR-TKI
R1 member_of Arg1:T3 Arg2:T2
~~~

~~~ ann
LOXL1/LOXL2 gene expression and protein levels were increased.
T1 GGPs 0 5 LOXL1
T2 GGPs 6 11 LOXL2
T5 Gene_expression 12 27 gene expression
T6 Gene_expression 12 27 gene expression
T7 Gene_expression 32 46 protein levels
T8 Gene_expression 32 46 protein levels
T9 Positive_regulation 52 61 increased
T10 Positive_regulation 52 61 increased
T11 Positive_regulation 52 61 increased
T12 Positive_regulation 52 61 increased
E1 Gene_expression:T5 Theme:T1
E2 Gene_expression:T6 Theme:T2
E3 Gene_expression:T7 Theme:T1
E4 Gene_expression:T8 Theme:T2
E5 Positive_regulation:T9 Theme:E1
E6 Positive_regulation:T10 Theme:E2
E7 Positive_regulation:T11 Theme:E3
E8 Positive_regulation:T12 Theme:E4
~~~

<!-- corrected 
~~~ ann
LOXL1/LOXL2 gene expression and protein levels were increased.
T1 GGPs 0 5;12 16 LOXL1 gene
T2 GGPs 6 16 LOXL2 gene
T3 GGPs 0 5;32 39 LOXL1 protein
T4 GGPs 6 11;32 39 LOXL2 protein
T5 Gene_expression 12 27 gene expression
T6 Gene_expression 12 27 gene expression
T7 Gene_expression 32 46 protein levels
T8 Gene_expression 32 46 protein levels
T9 Positive_regulation 52 61 increased
T10 Positive_regulation 52 61 increased
T11 Positive_regulation 52 61 increased
T12 Positive_regulation 52 61 increased
E1 Gene_expression:T5 Theme:T1
E2 Gene_expression:T6 Theme:T2
E3 Gene_expression:T7 Theme:T3
E4 Gene_expression:T8 Theme:T4
E5 Positive_regulation:T9 Theme:E1
E6 Positive_regulation:T10 Theme:E2
E7 Positive_regulation:T11 Theme:E3
E8 Positive_regulation:T12 Theme:E4
~~~
-->

~~~ ann
luciferase activity was elevated.
T1 GGPs 0 10 luciferase
T2 Positive_regulation 24 32 elevated
E1 Positive_regulation:T2 Theme:T1
~~~

~~~ ann
PLC inhibitor, U-73122
T1 GGPs 0 3 PLC
T2 Negative_regulation 4 13 inhibitor
T3 Pharmacological_substance 15 22 U-73122
E1 Negative_regulation:T2 Cause:T3 Theme:T1
~~~
~~~ ann
Rho inhibitor C3 exotoxin
T1 GGPs 0 3 Rho
T2 Negative_regulation 4 13 inhibitor
T3 GGPs 14 25 C3 exotoxin
E1 Negative_regulation:T2 Cause:T3 Theme:T1
~~~
~~~ ann
interleukin (IL)-33
T1 GGPs 0 11 interleukin
T2 GGPs 13 15 IL
T3 GGPs 0 11;16 19 interleukin-33
T4 GGPs 13 15;16 19 IL-33
R1 member_of Arg1:T3 Arg2:T1
R2 is_equivalent Arg1:T4 Arg2:T3
~~~

In case of modified GGPs, annotation can be performed as follows:
~~~ ann
Phospho-S6
T1 Conversion 0 7 Phospho
T2 GGPs 8 10 S6
T3 GGPs 0 10 Phospho-S6
E1 Conversion:T1 Theme:T2 Product:T3
~~~

Regarding *mutant/variant* information, it is extremely difficult to normalize them, as there are too many possible mutants for any GGPs. Thus, such *mutant/variant* information will be included in *Notes*, as follows:

- mutant C125A


For protein molecules, the <a href="https://proconsortium.org/pro/pro.shtml">PRO database (Protein Ontology)</a> in the <a href="https://proteininformationresource.org/">PIR database</a> are usually used for normalization in the other corpus.
On the other hand, the granularity of IDs from the <a href="https://www.uniprot.org/">UniProt database</a> is usually too small to use.
An example is indicated as follows:

<div style="margin:1em" markdown="1">

| Protein name |  UMLS ID    |      PRO ID      | UniProt ID |
|--------------|-------------|------------------|------------|
| Vascular endothelial growth factor A | C1823619 | PR:000017284 | - |
| VEGFA | C1823619 | PR:000017284 | - |
| human Vascular endothelial growth factor A | - | PR:P15692 | P15692 |
| hVEGFA | - | PR:P15692 | P15692 |

</div>

<a href="https://en.wikipedia.org/wiki/Chemokine">Chemokines</a>, such as IL-8, and <a href="https://en.wikipedia.org/wiki/Chemokine_receptor">their corresponding receptors</a>, which are composed of proteins, are categorized into this entity.

<div style="margin:1em" markdown="1">

| Protein name |  cells attracted by corresponding protein   | cytokine/receptor      | UMLS ID |
|--------------|----------------------|------------------|------------|
| CCL1   | T-lymphocytes  |  cytokine  | |
| CCL2   | Monocytes / macrophages / T-lymphocytes  |  cytokine  | |
| CCL3   | Monocytes / macrophages  |  cytokine  | |
| CCL5   | Monocytes / macrophages  |  cytokine  | |
| CCL7   | Monocytes / macrophages  |  cytokine  | |
| CCL8   | Monocytes / macrophages  |  cytokine  | |
| CCL13  | Monocytes / macrophages  |  cytokine  | |
| CCL17  | Monocytes / macrophages / T-lymphocytes  |  cytokine  | |
| CCL22  | Monocytes / macrophages / T-lymphocytes  |  cytokine  | |
| CCR1   | Mast cells   | receptor  | |
| CCR2   | Mast cells   | receptor  | |
| CCR3   | Mast cells   | receptor  | |
| CCR4   | Mast cells   | receptor  | |
| CCR5   | Mast cells   | receptor  | |
| CXCR2  | Mast cells   | receptor  | | 
| CXCR4  | Mast cells   | receptor  | |

</div>

<!-- details -->
