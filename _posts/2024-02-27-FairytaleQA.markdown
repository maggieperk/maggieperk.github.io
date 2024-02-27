---
layout: post
title:  "Question Generation for Reading Comprehension"
date:   2024-02-27 09:15:54 +0100
categories: projects
---
## Project Overview
The full details of this work are described in this [paper](https://aclanthology.org/2023.bea-1.47.pdf).

In recent decades, there has been a significant push to leverage technology to aid both teachers and students in the classroom. Language
processing advancements have been harnessed to provide better tutoring services, automated feedback to teachers, improved peer-to-peer
feedback mechanisms, and measures of student comprehension for reading. Automated question generation systems have the potential to
significantly reduce teachers’ workload in the latter. In this paper, we compare three different neural architectures for question generation
across two types of reading material: narratives and textbooks. For each architecture, we explore the benefits of including question attributes in the input representation. Our models show that a T5 architecture has the best overall performance, with a RougeL score of 0.536 on a narrative corpus and 0.316 on a textbook corpus. We break down the results by attribute and discover that the attribute can improve the quality of some types of generated questions, including Action and Character, but this is not true for all models.
## Authorship & Methodology
For this project, I created the training dataset for the question generation task based off of the Textbook Question Answering dataset[1].  I leveraged the correct answers from their set of multiple-choice style questions to create question-answer pairs and used the corresponding textbook section as the context to provide to a model.  For the experiments, I did all of the fine-tuning experiments with the T5-model [2].  I fine-tune the model in two different domains: the scientific domain from the Textbooking Question Answering corpus and the narrative domain using the FairytaleQA corpus [3].  I then evaluate the model using automated metrics as well as manually annotating the responses from all three of the models we use in the paper.

## Outcome
This work was presented as part of the 2023 Building Education Applications workshop co-located with ACL 2023 in Toronto, Canada.

## References
1. Aniruddha Kembhavi, Minjoon Seo, Dustin Schwenk, Jonghyun Choi, Ali Farhadi, and Hannaneh Hajishirzi. 2017. Are you smarter than a sixth grader? Textbook question answering for multimodal machine comprehension. In 2017 IEEE Conference on Computer Vision and Pattern Recognition (CVPR), Honolulu, HI. IEEE.
2. Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, and Peter J. Liu. 2019. Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer.
3. Ying Xu, Dakuo Wang, Mo Yu, Daniel Ritchie, Bingsheng Yao, Tongshuang Wu, Zheng Zhang, Toby Li, Nora Bradford, Branda Sun, Tran Hoang, Yisi Sang, Yufang Hou, Xiaojuan Ma, Diyi Yang, Nanyun Peng, Zhou Yu, and Mark Warschauer. 2022. Fantastic Questions and Where to Find Them: FairytaleQA -- An Authentic Dataset for Narrative Comprehension. In Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers), pages 447–460, Dublin, Ireland. Association for Computational Linguistics.
