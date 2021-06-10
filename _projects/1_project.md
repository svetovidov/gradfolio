---
layout: post
title: AI for Policy Making
description: Leveraging AI methods to provide recommendations for policy makers
---

Policies issued and adopted on a state and federal level have a significant effect on the lives of millions of people. At the same time, a lawmaking process itself is very time-consuming and imposes large human effort overhead. The goal of this study is to build a complete AI system to provide policymakers with recommendations on how a proposed law would affect the metric of interest.

We focused on predicting the impact of a given law text on internet broadband speed (excitatory/inhibitory). The main data source (law texts, internet speed) is a Federal Communications Commission [website](https://opendata.fcc.gov){:target="_blank"}. Additionally, contextual state-level data have been crawled to be used as features for training.

In this project, I worked on preprocessing and vectorizing raw texts of laws with GloVe embedding, as well as implementing machine learning models for policy classification, including random forests, logistic regression, multinomial Naive Bayes, and deep neural networks. The results were presented at a poster section of the FLAIRS conference and can be found [here](https://journals.flvc.org/FLAIRS/article/view/128499){:target="_blank"}

Project [repo](https://github.com/AI-VTRC/AIassurance){:target="_blank"}

*Tools used: Python, Scikit-learn, PyTorch, Git*