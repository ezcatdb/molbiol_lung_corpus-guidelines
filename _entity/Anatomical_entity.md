---
layout: entry
title: "Anatomical_entity"
shortdef: "Anatomical entities, including organs and tissues"
order: 12
---

The name of this entity group is based on <a href="https://en.wikipedia.org/wiki/Anatomical_terminology">Anatomical terminology</a>.

Organs, such as lung, and tissues above cells are categorized into this entity group.

This entity may be based on the following ontology databases:
- <a href="https://www.ebi.ac.uk/ols/ontologies/fma">FMA</a>
- <a href="https://www.ebi.ac.uk/ols/ontologies/uberon">UBERON</a>
- <a href="https://www.ebi.ac.uk/ols/search?ontology=ncit">NCIT</a>

Regarding the organ, such as lung, the following words/phrases can also be annotated.
- <a href="https://en.wikipedia.org/wiki/Respiratory_system">respiratory system</a>（呼吸器系）
- respiratory apparatus 
- ventilatory system（呼吸器系）
  - right lung
  - left lung
  - main bronchi
  - lobar bronchus
  - lingular division bronchi
  - trachea
  - diaphragm

~~~ ann
Squamous cell carcinoma of the lung invaded the right main bronchus.
T1 Disorder 0 23 Squamous cell carcinoma
T2 Cell 0 23 Squamous cell carcinoma
T3 Anatomical_entity 31 35 lung
T4 Anatomical_entity 48 67 right main bronchus
T5 Localization 36 43 invaded
E1 Localization:T5 Theme:T2 fromLoc:T3 toLoc:T4
~~~
~~~ ann
A 40-year-old man had undergone right upper lobectomy for lung cancer.
T1 Subject 2 17 40-year-old man
T3 Disorder 58 69 lung cancer
T5 Anatomical_entity 58 62 lung
R1 Subject_Disorder Arg1:T1 Arg2:T3
~~~
~~~ ann
The patient did not undergo lung resect.
T1 Subject 4 11 patient
T2 Negation_cue 16 19 not
T4 Anatomical_entity 28 32 lung
~~~
~~~ ann
Using PET-CT, we diagnosed liver metastases in the two patients.
T2 Anatomical_entity 27 32 liver
T4 Disorder 27 43 liver metastases
T5 Subject 51 63 two patients
T7 Localization 33 43 metastases
E2 Localization:T7 toLoc:T2
R1 Subject_Disorder Arg1:T5 Arg2:T4
~~~

Regarding tissues in lung, the following words/phrases can also be annotated.

- blood
- serum
- <a href="https://en.wikipedia.org/wiki/Pulmonary_alveolus">pulmonary alveolus</a>（肺胞）
- pulmonary alveoli（肺胞）
  - alveoli
  - atrium
  - pulmonary artery
  - pulmonary vein
  - alveolar sacs
  - alveolar duct
  - connective tissue
  - capillary beds
  - mucous gland
  - mucosal lining

- <a href="https://en.wikipedia.org/wiki/Pulmonary_pleurae">pulmonary pleurae</a>（胸膜）
  - parietal pleura


The following words/phrases are part of <a href="https://en.wikipedia.org/wiki/Circulatory_system">circulatory system</a>（循環器系）.

- aorta （大動脈）
  - ascending aorta
  - descending aorta
- 'vena cava' or 'venae cavae'（大静脈）
  - inferior vena cava
  - superior vena cava
- artery（動脈）
  - pulmonary artery
  - coronary artery
- vein（静脈）
  - pulmonary vein

<!-- details -->
