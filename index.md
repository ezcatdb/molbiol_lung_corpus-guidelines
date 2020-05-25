---
layout: entry
title: Annotation guidelines for molecuar biology corpus (lung diseases)
---

## Entities
- [General rules for entities](): {% assign i = site.entity | where_exp:"i", "i.title == 'General rules for entities'" | first %}{{ i.shortdef }}

## entities
<!--
- [Phenotype](): {% assign i = site.entity | where_exp:"i", "i.title == 'Phenotype'" | first %}{{ i.shortdef }}
-->

  - [Disorder](): {% assign i = site.entity | where_exp:"i", "i.title == 'Disorder'" | first %}{{ i.shortdef }}
    - [Measurement](): {% assign i = site.entity | where_exp:"i", "i.title == 'Measurement'" | first %}{{ i.shortdef }}
<!--
  - [Disease](): {% assign i = site.entity | where_exp:"i", "i.title == 'Disease'" | first %}{{ i.shortdef }}
  - [Symptom](): {% assign i = site.entity | where_exp:"i", "i.title == 'Symptom'" | first %}{{ i.shortdef }}
-->

- [Subject](): {% assign i = site.entity | where_exp:"i", "i.title == 'Subject'" | first %}{{ i.shortdef }}

<!--
  - [N_sbjct](): {% assign i = site.entity | where_exp:"i", "i.title == 'N_sbjct'" | first %}{{ i.shortdef }}
  - [Age_sbjct](): {% assign i = site.entity | where_exp:"i", "i.title == 'Age_sbjct'" | first %}{{ i.shortdef }}
  - [Ethnic_sbjct](): {% assign i = site.entity | where_exp:"i", "i.title == 'Ethnic_sbjct'" | first %}{{ i.shortdef }}
-->


- [Anatomical_entity](): {% assign i = site.entity | where_exp:"i", "i.title == 'Anatomical_entity'" | first %}{{ i.shortdef }}

<!--
- [Tissue_cultured](): {% assign i = site.entity | where_exp:"i", "i.title == 'Tissue_cultured'" | first %}{{ i.shortdef }}
- [Tissue_natural](): {% assign i = site.entity | where_exp:"i", "i.title == 'Tissue_natural'" | first %}{{ i.shortdef }}

- [Cell_cultured](): {% assign i = site.entity | where_exp:"i", "i.title == 'Cell_cultured'" | first %}{{ i.shortdef }}
- [Cell_natural](): {% assign i = site.entity | where_exp:"i", "i.title == 'Cell_natural'" | first %}{{ i.shortdef }}
-->

- [Cell](): {% assign i = site.entity | where_exp:"i", "i.title == 'Cell'" | first %}{{ i.shortdef }}
  - [Cell_component](): {% assign i = site.entity | where_exp:"i", "i.title == 'Cell_component'" | first %}{{ i.shortdef }}

- Molecular entities
  - [Pharmacological_substance](): {% assign i = site.entity | where_exp:"i", "i.title == 'Pharmacological_substance'" | first %}{{ i.shortdef }}
  - [GGPs](): {% assign i = site.entity | where_exp:"i", "i.title == 'GGPs'" | first %}{{ i.shortdef }}
  - [Inorganic_compound](): {% assign i = site.entity | where_exp:"i", "i.title == 'Inorganic_compound'" | first %}{{ i.shortdef }}
  - [Organic_compound_other](): {% assign i = site.entity | where_exp:"i", "i.title == 'Organic_compound_other'" | first %}{{ i.shortdef }}

<!--  
  - [Protein_molecule](): {% assign i = site.entity | where_exp:"i", "i.title == 'Protein_molecule'" | first %}{{ i.shortdef }}
  - [DNA_molecule](): {% assign i = site.entity | where_exp:"i", "i.title == 'DNA_molecule'" | first %}{{ i.shortdef }}
  - [RNA_molecule](): {% assign i = site.entity | where_exp:"i", "i.title == 'RNA_molecule'" | first %}{{ i.shortdef }}
-->

<!--  
- [Protein_family_or_group](): {% assign i = site.entity | where_exp:"i", "i.title == 'Protein_family_or_group'" | first %}{{ i.shortdef }}
-->

<!--  
    - [Amino_acid_monomer](): {% assign i = site.entity | where_exp:"i", "i.title == 'Amino_acid_monomer'" | first %}{{ i.shortdef }}
-->

<!--
- [Value](): {% assign i = site.entity | where_exp:"i", "i.title == 'Value'" | first %}{{ i.shortdef }}
  - [Dose](): {% assign i = site.entity | where_exp:"i", "i.title == 'Dose'" | first %}{{ i.shortdef }}
  - [Period](): {% assign i = site.entity | where_exp:"i", "i.title == 'Period'" | first %}{{ i.shortdef }}
-->

- [Entity Property](): {% assign i = site.entity | where_exp:"i", "i.title == 'Entity Property'" | first %}{{ i.shortdef }}

- [MENTION](): {% assign i = site.entity | where_exp:"i", "i.title == 'MENTION'" | first %}{{ i.shortdef }}

## cues
- [Negation Cue](): {% assign i = site.entity | where_exp:"i", "i.title == 'Negation Cue'" | first %}{{ i.shortdef }}
- [Speculation Cue](): {% assign i = site.entity | where_exp:"i", "i.title == 'Speculation Cue'" | first %}{{ i.shortdef }}

<!--  
- [Method Cue](): {% assign i = site.entity | where_exp:"i", "i.title == 'Method Cue'" | first %}{{ i.shortdef }}
-->

<!---
## additional
{% assign sorted = site.entity | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}
--->

## Events

- [Artificial_process](): {% assign i = site.event | where_exp:"i", "i.title == 'Artificial_process'" | first %}{{ i.shortdef }}
- [Biological_process](): {% assign i = site.event | where_exp:"i", "i.title == 'Biological_process'" | first %}{{ i.shortdef }}

  - [Localization](): {% assign i = site.event | where_exp:"i", "i.title == 'Localization'" | first %}{{ i.shortdef }}
  
  - [Regulation](): {% assign i = site.event | where_exp:"i", "i.title == 'Regulation'" | first %}{{ i.shortdef }}
    - [Negative_regulation](): {% assign i = site.event | where_exp:"i", "i.title == 'Negative_regulation'" | first %}{{ i.shortdef }}
    - [Positive_regulation](): {% assign i = site.event | where_exp:"i", "i.title == 'Positive_regulation'" | first %}{{ i.shortdef }}
    
  - [Cellular_process](): {% assign i = site.event | where_exp:"i", "i.title == 'Cellular_process'" | first %}{{ i.shortdef }}
    - [Molecular_function](): {% assign i = site.event | where_exp:"i", "i.title == 'Molecular_function'" | first %}{{ i.shortdef }}
      - [Pathway](): {% assign i = site.event | where_exp:"i", "i.title == 'Pathway'" | first %}{{ i.shortdef }}
          - [Conversion](): {% assign i = site.event | where_exp:"i", "i.title == 'Conversion'" | first %}{{ i.shortdef }}
      - [Gene_expression](): {% assign i = site.event | where_exp:"i", "i.title == 'Gene_expression'" | first %}{{ i.shortdef }}
      - [Binding](): {% assign i = site.event | where_exp:"i", "i.title == 'Binding'" | first %}{{ i.shortdef }}
      - [Dissociation](): {% assign i = site.event | where_exp:"i", "i.title == 'Dissociation'" | first %}{{ i.shortdef }}

    
<!-- Under Cellular process
    - [Migration](): {% assign i = site.event | where_exp:"i", "i.title == 'Migration'" | first %}{{ i.shortdef }} 
 -->

<!-- 
     - [Metabolism](): {% assign i = site.event | where_exp:"i", "i.title == 'Metabolism'" | first %}{{ i.shortdef }}
         - [Biosynthesis](): {% assign i = site.event | where_exp:"i", "i.title == 'Biosynthesis'" | first %}{{ i.shortdef }}
         - [Degradation](): {% assign i = site.event | where_exp:"i", "i.title == 'Degradation'" | first %}{{ i.shortdef }}
    - [Gene_expression](): {% assign i = site.event | where_exp:"i", "i.title == 'Gene_expression'" | first %}{{ i.shortdef }}
      - [Transcription](): {% assign i = site.event | where_exp:"i", "i.title == 'Transcription'" | first %}{{ i.shortdef }}
      - [Translation](): {% assign i = site.event | where_exp:"i", "i.title == 'Translation'" | first %}{{ i.shortdef }}
-->

<!---
{% assign sorted = site.event | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}
--->

## Relations

- [is_equivalent](): {% assign i = site.relation | where_exp:"i", "i.title == 'is_equivalent'" | first %}{{ i.shortdef }}
- [member_of](): {% assign i = site.relation | where_exp:"i", "i.title == 'member_of'" | first %}{{ i.shortdef }}
- [part_of](): {% assign i = site.relation | where_exp:"i", "i.title == 'part_of'" | first %}{{ i.shortdef }}
- [Subject_Disorder](): {% assign i = site.relation | where_exp:"i", "i.title == 'Subject_Disorder'" | first %}{{ i.shortdef }}

<!---
{% assign sorted = site.relation | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}
--->

## Attributes

- [Negated](): {% assign i = site.attribute | where_exp:"i", "i.title == 'Negated'" | first %}{{ i.shortdef }}
- [Speculated](): {% assign i = site.attribute | where_exp:"i", "i.title == 'Speculated'" | first %}{{ i.shortdef }}
  - [Certainty](): {% assign i = site.attribute | where_exp:"i", "i.title == 'Certainty'" | first %}{{ i.shortdef }}

- [Count_sbjct](): {% assign i = site.attribute | where_exp:"i", "i.title == 'Count_sbjct'" | first %}{{ i.shortdef }}

<!---
- [MutantAttribute](): {% assign i = site.attribute | where_exp:"i", "i.title == 'MutantAttribute'" | first %}{{ i.shortdef }}
- [Gender_sbjct](): {% assign i = site.attribute | where_exp:"i", "i.title == 'Gender_sbjct'" | first %}{{ i.shortdef }}
--->

<!--
{% assign sorted = site.attribute | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}
-->
