# Project Title

## About <a name = "about"></a>

This is the individual repository for UWA Capstone Project Group 7 : Machine Learning Estimation of In-Patient Metrics. This project aims to determine if machine learning can be applied to Australian healthcare problems.

- The objective of this repo is to determine if machine learning can predict whether a patient will die ahead of time.

## Getting Started <a name = "getting_started"></a>

### Prerequisites

All of the code implementations used Python 3.8.13 with Jupyter notebook IDE. The package dependencies are in requirements.txt

- Notice that different TensorFlow versions is used for different models since SHAP deepexplainer package is only compatible with TensorFlow 2.4.0 and above.

```
pip install -r requirements.txt
```

## Directory Structure

```
uwa-capstone-project-7-Tim/
┣ 0_EDA/
┃ ┣ figure/┃ ┃
┃ ┗ mort_data_prep.py.ipynb
┣ 1_TANML/
┃ ┗ mort_model.ipynb
┣ 2_TANL_SMOTE/
┃ ┗ mort_model_smote.ipynb
┣ 3_NN/
┃ ┣ mort_model_NN.ipynb
┃ ┣ shap_NN.ipynb
┃ ┗ Vital_sign.ipynb
┣ .gitignore
┣ README.md
┗ requirements.txt
```

### 0_EDA

- This folder contains the data preparation and exploratory data analysis (EDA) of the mortality dataset. The data preprocessing and EDA is done in the Jupyter notebook file mort_data_prep.py.ipynb. The figures generated from the EDA are stored in the figure folder.

### 1_TANML

- This folder contains the implementation of approach 1 (traditional machine learning models + no sampling). The implementation is done in the Jupyter notebook file mort_model.ipynb.

### 2_TANL_SMOTE

- This folder contains the implementation of approach 2 (traditional machine learning models + SMOTE sampling). The implementation is done in the Jupyter notebook file mort_model_smote.ipynb.

### 3_NN

- This folder contains the implementation of approach 3 (neural network models + no sampling). The implementation is done in the Jupyter notebook file mort_model_NN.ipynb.
- The SHAP deepexplainer is used to explain the neural network model. The implementation is done in the Jupyter notebook file shap_NN.ipynb.
- Thanks for group member Linh for providing the model structure of the neural network model. The implementation is done in the Jupyter notebook file Vital_sign.ipynb.
