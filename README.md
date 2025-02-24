# Introduction
Healthcare companies are increasingly using AI to lessen the burden on healthcare professionals, enhance healthcare services, analyze patient records, and cut costs. However, understanding the decision-making process of AI systems, particularly black box algorithms, can be challenging due to a lack of transparency. This lack of transparency can lead to inaccurate or biased findings, resulting in legal action, harm to the business's reputation, and loss of confidence in the use of black box algorithms. To ensure patients are willing to participate in clinical trials or receive personalized treatments, it's important that they understand how algorithms work and generate their findings. The study aims to assess current integrated XAI frameworks that can help reduce the use of opaque predictions in prostate cancer.

## Dataset Description
MedQuAD was created by Abacha and Demner-Fushman, (2019). It contains 47,457 medical question-answer pairs derived from 12 NIH websites (for example, cancer.gov, niddk.nih.gov, GARD, and MedlinePlus Health Topics). The collection includes 37 different sorts of questions addressing areas such as side effects, diagnosis, treatment and their connection with the various diseases, medications, and other medical tasks (JohnM, 2023). curated the dataset.


## Code Implementation
The MedQuAD dataset was uploaded to Google Colab and imported via the directory path. Due to the size of the data, a subset of the dataset had to be used for processing. This is because the explainers (particularly SHAP) take more time to explain. The focus area for the subset of the datasets selected were Breast Cancer and Prostate Cancer. In the pre-processing stage, the labels to be classified which are Breast Cancer and Prostate Cancer were assigned to a variable. Feature selection was also performed to identify the dependent and independent variables. The dependent variable was encoded using the label encoder function. The dataset was then split for training (80%) and testing (20%) and the class names were identified. The train split was transformed using the TFIDF() function.
