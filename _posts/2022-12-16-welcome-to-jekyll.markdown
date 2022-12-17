---
layout: post
title:  "BST 260 Final Project"
date:   2022-12-16 20:48:21 -0500
categories: jekyll update
---

Project Overview: 

Using the ICU data included in the MIMIC-IV database sourced from Beth Israel Deaconess Medical Center mortality was predicted using laboratory results returned in the first 24 hours of the patient's stay in the ICU. 
To predict mortality, both logisitc regression and random forest models were generated and top predicitve features from both models were determined. 
Comparing the results of both models, the logisitic regression had higher overall scores. The top predictive features include lactate, sodium, and albumin levels. 

Results: 
For logistic regression and random forest model a training and testing datasets were generated with a 80/20 split. Logistic regression modeling was performed and tested with an accuracy of 0.74, indicating that the model was able to correctly identify patients that were at risk for mortality 74% of the time. The logistic regression model also reported a sensitivity or recall score of 0.76  and specificity of 0.71 showing 76% of the time mortality was predicted correctly and 71% of the time survival was predicted correctly. Using the ‘vip’ package in r the variable importance was plotted for the logistic regression model [5]. The plot shows, ‘albumin_min’, ‘lactate_max’, ‘lactate_min’, and ‘sodium_max’ as the top predictive features of mortality for MIMIC-IV ICU patients. Finally, the ROC-AUC curve was plotted for the logistic regression model and reported an AUC of 0.74. This value closely matches the accuracy of the model and provides additional evidence of the predictive qualities of the model. 

Conclusion:
The goal of this study was to report the predictive properties of laboratory results of MIMIC-IV patients in the ICU on the outcome of mortality. The features were evaluated using logistic regression and random forest modeling to determine the relative importance of each feature as well as the function of the mortality prediction model overall. While the logistic regression model did have a lower overall accuracy compared to the random forest, there was more even balance in the sensitivity and specificity metrics. In the case of mortality prediction in the ICU there is greater concern in a low sensitivity as that would indicate a low ability to predict mortality which has a greater consequence than low specificity, indicating reduced survival prediction.
 
 Both models found that the lactate variable is highly predictive of mortality. As well as lactate, both models selected sodium as an important variable for predicting mortality. These results are in line with current medical understanding. Changes in lactate are often noted as the onset for changes in blood pressure and heart rate which are important indicators of health [6]. Lactate levels have also been reported to correlate with the diagnosis of septic shock in critically ill patients [7].  High sodium levels have also been reported to indicate renal function decline and dehydration which both are important for patient health [8,9]. The top predictive features selected  by both models are not surprising and give greater evidence that the predictive model is informative of patient health within the first 24 hours of lab results collected

Flow Chart of subject selection into the study from the MIMIC-IV database:

![Flow-Chart](https://github.com/zoe-love/BST-260-Final-Project/blob/main/FlowChart.png?raw=true "Subject Selection Flow Chart")

Table 1:
![Table-One](https://github.com/zoe-love/BST-260-Final-Project/blob/main/Table%201.png?raw=true "Table One")

Model Evaluation:
![Eval-Model](https://github.com/zoe-love/BST-260-Final-Project/blob/main/Eval%20Table.png?raw=true "Eval")

ROC-AUC Curve for Logistic Regression Model:
![ROC-AUC](https://github.com/zoe-love/BST-260-Final-Project/blob/main/ROC_AUC.png?raw=true "ROC-AUC")

Top Predictive Features Selected by Logistic Regression Model:
![VIP](https://github.com/zoe-love/BST-260-Final-Project/blob/main/VIP_log.png?raw=true "VIP Log")
