# BST-260-Final-Project
Evaluation of top predictive lab variables for mortality in MIMIC-IV patients

Pipeline of analysis for reproducibility:

1. Extract MIMIC-IV SQL tables in Google Colab notebook 'Final_Project_Data_Extraction.ipynb' to generate 'ICU_df.csv'

2. Run the 'Final Report.rmd' to generate the report. Must have 'FlowChart.png' in directory to run fully. 

3. To generate the full report I submitted you must also extract the 'untidy' version of the dataset, however, this dataset is over 25 MB. 
Therefore, I cannot upload it to github as it is too large. This will cause an issue if you attempt to knit the 'Final Report.rmd'
I am inlcuding 'Final Report Small.rmd' file that does not require the original untidy data. You can knit that from your computer. 
