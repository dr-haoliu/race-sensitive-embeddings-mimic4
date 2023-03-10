# race-sensitive-embeddings-mimic4

## Source code repo for  AMIA Informatics Summit 2023 paper `Can Race-sensitive Biomedical Embeddings Improve Healthcare Predictive Models`

## Please cite the paper and give a star if you use the code in this repo. 

## Abstract
This reproducibility study presents an algorithm to weigh in race distribution data of clinical research study samples when training biomedical embeddings.   
We extracted 12,864 PubMed abstracts published between January 1st, 2000 and January 1st, 2022 and weighed them based on the race distribution data extracted from their corresponding clinical trials registered on ClinicalTrials.gov.   
We trained Word2vec and BERT embeddings and evaluated their performance on predicting length of hospital stay (LHS) and intensive care unit (ICU) readmission using MIMIC-IV electronic health record data.  
We observed that models trained using race-sensitive embeddings do not consistently outperform the neutral embeddings ones when used for LHS prediction (with similar Mean Absolute Error 1.975 vs. 2.008) or ICU readmission prediction (with similar accuracy 74.61% vs. 75.17% and the same AUC 0.775), respectively.   
We conclude that demographic sensitive embeddings do not necessarily significantly improve the accuracy of health predictive models as previously reported in the literature.  




## Installation & Usage
+ [download clinical trials and pubmed abstracts](download_clinical_trials_and_pubmed_abstracts.ipynb)
+ [train FastText embeddings](train_embeddings_fasttext.ipynb)
+ [train BERT embeddings](train_embeddings_BERT.ipynb)
+ [generate ICU readmission and Length of hospital stay data from mimic4 ](generate_mimic4_stay_icu_readmission_data.ipynb)
+ [test neutral BERT embeddings for ICU readmission and Length of hospital stay prediction](Prediction_BERT_embedding_test_neutral.ipynb)
+ [test race-sensitive BERT embeddings for ICU readmission and Length of hospital stay prediction](Prediction_BERT_embedding_test_sensitive.ipynb)
+ [test neutral and race-sensitive FastText embeddings for ICU readmission](Prediction_FastText_embedding_test_Readmission.ipynb)
+ [test neutral and race-sensitive FastText embeddings for Length of hospital stay prediction](Prediction_FastText_embedding_test_LOS.ipynb)


## License
This project is licensed under the terms of the MIT license.
