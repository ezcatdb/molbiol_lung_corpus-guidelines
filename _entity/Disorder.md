---
layout: entry
title: "Disorder"
shortdef: "Disorders"
order: 2
---

The definition of 'Disorder' is based on the Semantic types of 
- 'dsyn' (Disease or Syndrome),
- 'neop' (Neoplastic Process), 
- 'patf' (Pathologic Function), and
- 'sosy' (Sign or Symptom) 

in the <a href="https://www.nlm.nih.gov/research/umls/">UMLS database</a>.

<!--
 <a href="https://icd.who.int/browse11/l-m/en">ICD-11</a> published by WHO,
although <a href="http://apps.who.int/classifications/icd10/browse/2016/en">ICD-10 version:2016</a> has been more widely used than ICD-11.
-->

Diseases and symptoms, which can be a group in phenotype, will be annotated in this category. 

~~~ ann
Idiopathic pulmonary fibrosis (IPF) is a fatal condition. 
T1 Disorder 0 29 Idiopathic pulmonary fibrosis
T2 Disorder 31 34 IPF
T3 Disorder 41 56 fatal condition
~~~

~~~ ann
A 40-year-old man had undergone right upper lobectomy for lung cancer.
T1 Subject 2 17 40-year-old man
T2 Artificial_process 32 53 right upper lobectomy
T3 Disorder 58 70 lung cancer
E1 Artificial_process:T2 Theme:T1
R1 Subject_Disorder Arg1:T1 Arg2:T3
~~~

The following words/phrases should be annotated as 'Disorder'.

- lung cancer 
- lung adenocarcinoma 
- non-small cell lung cancer 
- multiple myeloma 
- plasma cell myeloma 
- chronic obstructive pulmonary disease 
- COPD 
- acute exacerbation of chronic obstructive pulmonary disease 
- AECOPD 
- bronchiolitis obliterans (syndrome) 
- idiopathic pulmonary fibrosis 
- IPF 
- idiopathic interstitial pneumonia 
- interstitial lung disease 
- pulmonary hypertension 
- sarcoidosis 
- pulmonary sarcoidosis 
- pleural effusion 
- lung lesions 
- allodynia 


<!--
<div style="margin:1em" markdown="1">

| Disease name | ICD-10 code | ICD-10 description | ICD-11 code | ICD-11 description |
|--------------------------------------|-------------|------------------------------------------|-------------|------------------------------------------|
| lung cancer | C34 | Malignant neoplasm of bronchus and lung | 2C25 | Malignant neoplasms of bronchus or lung |
| lung adenocarcinoma | - | - | 2C25.0 | Adenocarcinoma of bronchus or lung |
| non-small cell lung cancer | - | - | 2C25.Y | Other specified malignant neoplasms of bronchus or lung |
| multiple myeloma | C90.0 | Multiple myeloma | 2A83.1 | Plasma cell myeloma |
| plasma cell myeloma | C90.0 | Multiple myeloma | 2A83.1 | Plasma cell myeloma |
| chronic obstructive pulmonary disease | J44 | Other chronic obstructive pulmonary disease | CA22 | Chronic obstructive pulmonary disease |
| COPD | J44 | Other chronic obstructive pulmonary disease | CA22 | Chronic obstructive pulmonary disease |
| acute exacerbation of chronic obstructive pulmonary disease | J44.1 | Chronic obstructive pulmonary disease with acute exacerbation, unspecified | CA22.0 | Chronic obstructive pulmonary disease with acute exacerbation, unspecified  |
| AECOPD | J44.1 | Chronic obstructive pulmonary disease with acute exacerbation, unspecified | CA22.0 | Chronic obstructive pulmonary disease with acute exacerbation, unspecified  |
| bronchiolitis obliterans (syndrome) | J44.8 | Other specified chronic obstructive pulmonary disease  | CA26.Z | Chronic bronchiolitis, unspecified |
| idiopathic pulmonary fibrosis | J84.1 | Other interstitial pulmonary diseases with fibrosis | CB03.4 | Idiopathic pulmonary fibrosis |
| IPF | J84.1 | Other interstitial pulmonary diseases with fibrosis | CB03.4 | Idiopathic pulmonary fibrosis |
| idiopathic interstitial pneumonia | J84.1 | Other interstitial pulmonary diseases with fibrosis | CB03.Z | Idiopathic interstitial pneumonitis, unspecified |
| interstitial lung disease | J84.9 | Interstitial pulmonary disease, unspecified | CB0? | Respiratory diseases principally affecting the lung interstitium |
| pulmonary hypertension | I27.0, I27.2 | Primary pulmonary hypertension, Other secondary pulmonary hypertension | BB01 | Pulmonary hypertension |
| Sarcoidosis | D86 | Sarcoidosis | 4B20 | Sarcoidosis |
| pulmonary sarcoidosis | D86.0 | Sarcoidosis of lung | 4B20.0 | Sarcoidosis of lung |
| pleural effusion | - | - | CB27 | Pleural effusion |
| lung lesions | R91 | Abnormal findings on diagnostic imaging of lung | MD41 | Clinical findings on diagnostic imaging of lung |
| allodynia | - | - | MB40.1 | Allodynia |


</div>
-->

<div style="background-color: yellow" markdown="1">
Some disease names start with 'AE (acute exacerbation)'. As these words suggest the change in disorder entities, 'Disorder', they may be annotated as event entity, [Biological_process]():
- acute exacerbation of idiopathic pulmonary fibrosis
- AE-IPF

</div>

~~~ ann
The pathogenesis of acute exacerbations of idiopathic pulmonary fibrosis (AE-IPF)
T1 Biological_process 20 39 acute exacerbations
T2 Disorder 43 72 idiopathic pulmonary fibrosis
T3 Biological_process 74 76 AE
T4 Disorder 77 80 IPF
R3 is_equivalent Arg1:T4 Arg2:T2
R4 is_equivalent Arg1:T3 Arg2:T1
~~~

<!--
The following words/phrases, whose ICD-10 IDs start with R, or whose ICD-11 IDs start with M, may be annotated as [Symptom](). 
<div style="margin:1em" markdown="1">

| Disease name | ICD-10 code | ICD-10 description | ICD-11 code | ICD-11 description |
|--------------------------------------|-------------|------------------------------------------|-------------|------------------------------------------|
| lung lesions | R91 | Abnormal findings on diagnostic imaging of lung | MD41 | Clinical findings on diagnostic imaging of lung |
| allodynia | - | - | MB40.1 | Allodynia |

</div>
-->

Symptoms, which can be a group in phenotype, will be annotated in this category. 
The following words/phrases should be annotated as 'Disorder'.

- breathing disorder
  - sleep breathing disorder
- rash
- diarrhea
- hematologic toxicity

~~~ ann
The impact of IPF-related sleep breathing disorders (SBDs) on survival.
T1 Disorder 14 17 IPF
T2 Disorder 26 51 sleep breathing disorders
T3 Disorder 53 57 SBDs
R1 is_equivalent Arg1:T3 Arg2:T2
~~~
~~~ ann
The common adverse effects of Icotinib were rash and diarrhea.
T2 Pharmacological_substance 30 38 Icotinib
T3 Disorder 44 48 rash
T4 Disorder 53 61 diarrhea
~~~

- fatal condition

~~~ ann
Idiopathic pulmonary fibrosis (IPF) is a fatal condition. 
T1 Disorder 0 29 Idiopathic pulmonary fibrosis
T2 Disorder 31 34 IPF
T3 Disorder 41 56 fatal condition
~~~

<div style="background-color: yellow" markdown="1">
Regarding the image observation, the following phrases can be 'Disorder':
- ground glass
- ground-glass
- ground glass opacity
- ground-glass opacity
- ground glass opacification
- ground-glass opacification

</div>

<div style="background-color: yellow" markdown="1">
The following phrases also can be 'Disorder':

- chronic lung allograft dysfunction 
- restrictive allograft syndrome 
</div>

If the words, which indicate ambiguous degree/state, are not included in the UMLS data, the UMLS IDs should be selected for the disease themselves.
- IPF (UMLS; C1800706)
- advanced "IPF" (UMLS; C1800706)

<!--
~~~ ann
Patients with advanced IPF
T1 Subject 0 8 Patients
T2 Disorder 23 26 IPF
T3 Entity_Property 14 22 advanced
R1 Subject_Disorder arg1:T1 arg2:T2
N1	Reference T2 UMLS:C1800706	Idiopathic Pulmonary Fibrosis
~~~
-->

~~~ ann
Patients with advanced IPF
T1 Subject 0 8 Patients
T2 Disorder 23 26 IPF
T3 Entity_Property 14 22 advanced
T4 Disorder 14 26 advanced IPF
R1 Subject_Disorder arg1:T1 arg2:T4
R2 member_of arg1:T4 arg2:T2
N1	Reference T2 UMLS:C1800706	Idiopathic Pulmonary Fibrosis
~~~

The following words/phrases for stage/degree of disease are nnotated as [Entity Property]().
- stage I
- stage II
- stage IIIB
- stage IV
- stage IIIB/IV
- advanced (UMLS; C0205179)
- severe (UMLS; C0205082)

<!-- details -->
