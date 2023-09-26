# Staging Breast Cancer Using Conversational Retrieval
This project aims to develop a framework that uses Large Language Models (LLMs) to stage breast cancer based on the radiology and pathology reports. Here is the general framework:
<p align="center">
  <img src="https://github.com/laithomari/breast_cancer_staging/assets/54318618/8f03600a-4caf-4d8b-ba10-3045d7f93a45.png" width="725" height="910" />
</p>
The retrieval pipeline is based on indexing. Each merged note will be split to multiple chunks and each chunk will then be embedded. These embeddings will then be stored on a vector database. Then, a conversational retrieval will be used to incorporate only relevant chunks using similarity search, as shown in the following figure: 
<p align="center">
  <img src="https://github.com/laithomari/breast_cancer_staging/assets/54318618/f13961f6-7002-41e2-ac3b-781d42444761.png" width="725" height="1159" />

  # Machine Learning to Predict the Development of Atrial Fibrillation in Critically Ill Patients

This is the repository for our recent project that uses machine learning to predict atrial fibrillation in critically ill patients. We used data from the Medical Information Mart for Intensive Care (MIMIC-IV) database. The model achieved an area under the receiver operator characteristic curve (AUC) of 0.850. A compact model using 15 features in addition to 2 newly engineered features achieved a comparable AUC of 0.820.

<p align="center">
  <img src="https://github.com/laithomari/machine_learning_afib_prediction/assets/54318618/d601a780-033e-4b13-b95a-4940b7089796.png" width="600" height="500" />
</p>

The newly added features were the following:

1. **Older septic**: a categorical feature indicating if the patient is 70 years old or older and is septic.
2. **Cardiac risk score**: a score that incorporates patient's preexisting cardiac related risk factors:

<p align="center">
  <img src="https://github.com/laithomari/machine_learning_afib_prediction/assets/54318618/4627f18c-c775-462a-93fd-8552476fd6cc.png" />
</p>

Based on the Shapley Additive exPlanations (SHAP) analysis, the two newly engineered features, _older septic_ and _cardiac risk score_, were the second and third most influential features on model performance, respectively.

<p align="center">
  <img src="https://github.com/laithomari/machine_learning_afib_prediction/assets/54318618/eebfa8c4-1456-4e0d-80a6-27e0c550067c.png" width="600" height="622" />
</p>
