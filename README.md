# DenseCMT

Advancements of Vision Transformers (ViTs) with Convolutional Neural Networks Meet Vision Transformers (CMTs) increased their scope in solving various problems. Though CMTs capture long-range relationships and locally-centered features through convolutions, their performance on CT-Scan datasets for covid detection is limited on smaller datasets. The reasons are - lack of significant spatial feature extraction, weak intra-patch knowledge extraction, and the inability to capture scaled lesions. To overcome these issues, in this paper, we present DenseCMT - a wide hybrid model of CMTs and pre-trained DenseNet to combine knowledge of both. Our approach significantly enhances the model's performance on SARS COVID 2 CT SCAN dataset and Extensive COVID-19 X-ray and CT chest images dataset resulting in 98.99% and 98.64% accuracy,  respectively, surpassing both standalone CMT and DenseNet models. This demonstrates that transfer learning with DenseNet complements well with the CMT wide model in Covid detection.

# Datasets used
* SARS-CoV-2 Dataset  https://www.kaggle.com/datasets/plameneduardo/sarscov2-ctscan-dataset
* Extensive COVID-19 X-Ray and CT Chest Images Dataset  https://data.mendeley.com/datasets/8h65ywd2jr

# Block Diagram
![overview_proposed](https://user-images.githubusercontent.com/75313778/224008118-66fa5f1b-105d-4c5a-9601-825b64a6ba3e.jpg)

Dataset  | Proposed Method | Loss | Accuracy | Precision | Recall | F1-score | Sensitivity | Specificity
------------- | -------------
SARS-CoV-2  | DenseCMT (CMT_2345 + DenseNet169) | 0.0472	|	98.99	|	0.99	|	0.9899	|	0.9899	|	0.996	|	0.9837
Extensive COVID-19 X-Ray and CT Chest  | DenseCMT (CMT_2345 + DenseNet121) | 0.0467	|	98.64	|	0.9864	|	0.9864	|	0.9864	|	0.989	|	0.981

