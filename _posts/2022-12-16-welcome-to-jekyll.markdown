---
layout: post
title:  "BST 260 Final Project"
date:   2022-12-16 20:48:21 -0500
categories: jekyll update
---

Project Description: 

Using the ICU data included in the MIMIC-IV database sourced from Beth Israel Deaconess Medical Center mortality was predicted using laboratory results returned in the first 24 hours of the patient's stay in the ICU. 
To predict mortality, both logisitc regression and random forest models were generated and top predicitve features from both models were determined. 
Comparing the results of both models, the logisitic regression had higher overall scores. The top predictive features include lactate, sodium, and albumin levels. 

Flow Chart of subject selection into the study from the MIMIC-IV database:

![Flow-Chart](https://github.com/zoe-love/BST-260-Final-Project/blob/main/FlowChart.png?raw=true "Subject Selection Flow Chart")

ROC-AUC Curve for Logistic Regression Model:
![ROC-AUC](https://github.com/zoe-love/BST-260-Final-Project/blob/main/ROC_AUC.png?raw=true "ROC-AUC")
