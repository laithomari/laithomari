# Staging Breast Cancer Using Conversational Retrieval
This project aims to develop a framework that uses Large Language Models (LLMs) to stage breast cancer based on the radiology and pathology reports. Here is the general framework:
<p align="center">
  <img src="https://github.com/laithomari/breast_cancer_staging/assets/54318618/8f03600a-4caf-4d8b-ba10-3045d7f93a45.png" width="725" height="910" />
</p>
The retrieval pipeline is based on indexing. Each merged note will be split to multiple chunks and each chunk will then be embedded. These embeddings will then be stored on a vector database. Then, a conversational retrieval will be used to incorporate only relevant chunks using similarity search, as shown in the following figure: 
<p align="center">
  <img src="https://github.com/laithomari/breast_cancer_staging/assets/54318618/f13961f6-7002-41e2-ac3b-781d42444761.png" width="725" height="1159" />
