# Credit Risk Analysis

## Purpose of Analysis:

The purpose of this project is to evaluate several machine learning models in order to predict credit risk. We will then analyze each model's performance and determine if each model is viable and make recommendations based on the analysis.

## Results

### RandomOverSampler model:

<img width="429" alt="Screenshot 2023-01-02 at 3 29 06 PM" src="https://user-images.githubusercontent.com/58227052/210275716-65a166b9-a0a6-4df5-a20b-c9a47f319ea4.png">

<img width="385" alt="Screenshot 2023-01-02 at 3 29 32 PM" src="https://user-images.githubusercontent.com/58227052/210275723-e10935ca-cd6c-48bf-b735-8a9bf5c33a72.png">

<img width="670" alt="Screenshot 2023-01-02 at 3 29 39 PM" src="https://user-images.githubusercontent.com/58227052/210275727-d47fded1-7747-413b-bda5-340ae752f3dc.png">

The balanced accuracy score is 62% with the high risk at only 1% and the low risk at 100%. High risk and low risk sensitivities are 59% and 69% respectively.


### SMOTE Oversampling model:

<img width="337" alt="Screenshot 2023-01-02 at 3 31 15 PM" src="https://user-images.githubusercontent.com/58227052/210275823-83204577-78e8-4b50-a192-79e627f0968b.png">

<img width="376" alt="Screenshot 2023-01-02 at 3 31 22 PM" src="https://user-images.githubusercontent.com/58227052/210275829-7bec8d44-1c47-4240-b3db-7d0db831a83c.png">

<img width="666" alt="Screenshot 2023-01-02 at 3 31 28 PM" src="https://user-images.githubusercontent.com/58227052/210275833-0e404ab9-42a5-44b5-8bac-cece0bf613a2.png">

The balanced accuracy score is 64% with the high risk at only 1% and the low risk at 100%. High risk and low risk sensitivities are 59% and 66% respectively.


### ClusterCentroids resampler model:

<img width="341" alt="Screenshot 2023-01-02 at 3 33 39 PM" src="https://user-images.githubusercontent.com/58227052/210276033-611f9892-9b8e-4e42-b8aa-909ce1a2f966.png">

<img width="379" alt="Screenshot 2023-01-02 at 3 33 47 PM" src="https://user-images.githubusercontent.com/58227052/210276042-5fcc876b-14ad-4010-800a-fd93e8c65998.png">

<img width="667" alt="Screenshot 2023-01-02 at 3 33 53 PM" src="https://user-images.githubusercontent.com/58227052/210276056-9e84cf59-6f67-4eb9-959f-1c57ee03b6b2.png">

The balanced accuracy score is 51% with the high risk at only 1% and the low risk at 100%. High risk and low risk sensitivities are 59% and 43% respectively.


### SMOTEENN model:

<img width="333" alt="Screenshot 2023-01-02 at 3 36 08 PM" src="https://user-images.githubusercontent.com/58227052/210276217-1c632a6f-e354-42f9-a84a-9d5610e34745.png">

<img width="375" alt="Screenshot 2023-01-02 at 3 36 14 PM" src="https://user-images.githubusercontent.com/58227052/210276222-ab7b25b7-e62c-4662-a34f-5aecfc64d5f1.png">

<img width="667" alt="Screenshot 2023-01-02 at 3 36 21 PM" src="https://user-images.githubusercontent.com/58227052/210276225-2c6b283d-6858-4b25-a071-8e6c2b444488.png">



### BalancedRandomForestClassifier model:

<img width="422" alt="Screenshot 2023-01-02 at 3 38 18 PM" src="https://user-images.githubusercontent.com/58227052/210276365-24c67cb8-91cc-4984-9164-b625fc5b1c90.png">

<img width="373" alt="Screenshot 2023-01-02 at 3 38 26 PM" src="https://user-images.githubusercontent.com/58227052/210276373-9e3c78c5-31d7-4a70-bf3e-be3ba4a22bb4.png">

<img width="668" alt="Screenshot 2023-01-02 at 3 38 33 PM" src="https://user-images.githubusercontent.com/58227052/210276385-0323fc5b-08ac-4641-a05e-da6e603d54d5.png">

The balanced accuracy score is 79% with the high risk at 4% and the low risk at 100%. High risk and low risk sensitivities are 67% and 91% respectively.

### EasyEnsembleClassifier model:

<img width="337" alt="Screenshot 2023-01-02 at 3 39 30 PM" src="https://user-images.githubusercontent.com/58227052/210276472-b9f17a43-be62-4f4f-b4aa-036fb11f049d.png">

<img width="378" alt="Screenshot 2023-01-02 at 3 39 37 PM" src="https://user-images.githubusercontent.com/58227052/210276477-be8a5fe8-5a7a-4705-9b8a-3d8f6dd053cf.png">

<img width="673" alt="Screenshot 2023-01-02 at 3 39 44 PM" src="https://user-images.githubusercontent.com/58227052/210276482-d5f23d05-a0b5-41a7-b652-a15940cb0cfb.png">

The balanced accuracy score is 93% with the high risk at 7% and the low risk at 100%. High risk and low risk sensitivities are 91% and 94% respectively.

## Summary

Unfortunately, all of our models show poor precision, although as you move towards the EasyEnsembleClassifier (EEC) model there is a noteable increase to precision sensitivity. The EEC model shows that it is detecting almost all high-risk credit but with the low precision value of 7% it is almost certainly lumping in some low-risk credit with the high-risk credit which would more than likely do more harm than good from a business perspective. Based on my understanding of the data I cannot actually recommend any of these models for prediciting credit risk. 
