---
layout: entry
title: "Speculation Cue"
shortdef: "speculation words and phrases"
order: 108
---

In addition to verbs, such as “suggest”, “show”, and “indicate”, the
following phrases can be speculation cues.

- can/could ***(be) (concluded/considered/described/interpreted/rationalized)***
- may/might
- Analyze(d/s)/analyse(d/s)
- Implication   
- Insight(s)
- Proposal(s)
- probability
- ~ consistent with
- ~ agree(s) (well) with
- ~ appear(s) ***(likely/favorable/to involve)***
- Argue against
- apparent/apparently
- understand(ing)
- hypothesize
- suggestive (of)
- Putative
- Presumably/probably
- presume(d)

~~~ ann
We hypothesized that direct implantation might have led to metastasis.
T1 Speculation_cue 3 15 hypothesized
T2 Surgery 21 40 direct implantation
T3 Speculation_cue 41 46 might
T4 Adverse_effect 52 58 led to
T5 Disease 59 69 metastasis
E1 Surgery:T2 
E2 Adverse_effect:T4 has_agent:E1 affects:T5 cue:T3 cue2:T1 
A1 Speculated E2
~~~

The following words indicate that the events involved are not clear/known.
- unclear
- unknown

The following words indicate that the events involved are tested/investigated. Thus, the events involved have not been confirmed yet.
- test(ed)
- investigate(d)/investigation
- evaluate(d)/evaluation
- measure(d)/measurement
- assess(ed)/assessment

~~~ ann
Markers of fibrogenesis, including collagen and CTGF were evaluated by measuring mRNA level using RT-PCR.
T1 GGPs 0 7 Markers
T2 Biological_process 11 23 fibrogenesis
T3 GGPs 35 43 collagen
T4 GGPs 48 52 CTGF
T5 Speculation_cue 58 67 evaluated
T6 Speculation_cue 71 80 measuring
T7 Gene_expression 81 91 mRNA level
T8 Gene_expression 81 91 mRNA level
T9 Method_cue 98 104 RT-PCR
E1 Biological_process:T2 Participant:E2 Participant2:E3 cue:T5
E2 Gene_expression:T7 Theme:T3 cue:T6 cue2:T9
E3 Gene_expression:T8 Theme:T4 cue:T6 cue2:T9
R1 member_of Arg1:T3 Arg2:T1
R2 member_of Arg1:T4 Arg2:T1
A1 Speculated E1
A2 Speculated E2
A3 Speculated E3
~~~

<!--details-->
