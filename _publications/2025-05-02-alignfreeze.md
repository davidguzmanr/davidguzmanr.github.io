---
title: "ALIGNFREEZE: Navigating the Impact of Realignment on the Layers of Multilingual Models Across Diverse Languages."
collection: publications
permalink: /publication/2025-05-alignfreeze
excerpt: "Realignment techniques are often employed to enhance cross-lingual transfer in multilingual language models, still, they can sometimes degrade performance in languages that differ significantly from the fine-tuned source language. This paper introduces AlignFreeze, a method that freezes either the layers’ lower half or upper half during realignment. Through controlled experiments on 4 tasks, 3 models, and in 35 languages, we find that realignment affects all the layers but can be the most detrimental to the lower ones. Freezing the lower layers can prevent performance degradation. Particularly, AlignFreeze improves Part-of-Speech (PoS) tagging performances in languages where full realignment fails: with XLM-R, it provides improvements of more than one standard deviation in accuracy in seven more languages than full realignment."
date: 2025-05-02
venue: "NAACL"
paperurl: "https://aclanthology.org/2025.naacl-short.48/"
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

**Abstract**

Realignment techniques are often employed to enhance cross-lingual transfer in multilingual language models, still, they can sometimes degrade performance in languages that differ significantly from the fine-tuned source language. This paper introduces AlignFreeze, a method that freezes either the layers’ lower half or upper half during realignment. Through controlled experiments on 4 tasks, 3 models, and in 35 languages, we find that realignment affects all the layers but can be the most detrimental to the lower ones. Freezing the lower layers can prevent performance degradation. Particularly, AlignFreeze improves Part-of-Speech (PoS) tagging performances in languages where full realignment fails: with XLM-R, it provides improvements of more than one standard deviation in accuracy in seven more languages than full realignment.

[Download paper here](https://aclanthology.org/2025.naacl-short.48/).
