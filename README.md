# Fake News Detection Using Machine Learning Models

An automated system that helps users to detect fake news articles.

---


## Overview

This code detects fake news through a text-based analysis, utilizing machine learning models and word embedding techniques. 

Traditional machine learning and deep learning models are trained to classify the text as either fake or true. They are trained individually and as hybrid models.

Accuracy is used to measure the model performance. 

---

## Installation

This code was written and run on Kaggle without the use of any kind of accelerator.

To run this project, make sure Python 3.7+ is installed.

If not, install all required modules using the following command:

- ###### pip install pandas numpy scipy nltk scikit-learn xgboost lightgbm matplotlib seaborn torch keras tensorflow

Be sure to also download the dataset and the word embedding technique (GloVe) files before running the code. The code would not be able to run otherwise. 

Due to its large size, the files are only available via the OneDrive links provided in the repository.

- Dataset: Download the dataset from "Dataset_onedrive_link.txt".
- GloVe: Download the file from "GloVe_onedrive_link.txt".

![image](https://github.com/user-attachments/assets/c4a780b7-c6a2-49b4-83ef-692709c469a1)

### NOTE: change the Dataset and GloVe files in the code to your personal path to ensure the code runs. 

---

## Usage

To run the automated system to detect fake news successfully:
1. Download the above files (dataset and GloVe).
2. Download the code .ipynb file - "Final Code - Detect Fake News.ipynb"
3. Download required models if needed. 
4. Update the file path in parts 1 and 3 of the code.
5. Run the code.
6. Observe the findings. 

![part 1](https://github.com/user-attachments/assets/3d343cfb-856f-4473-a0d5-0240a296c289)
![part 3](https://github.com/user-attachments/assets/34891fec-77b2-4d1b-96d9-cb858cdd4e8c)

---

## Code explanation

The code is made up of 9 parts. The details of each part are explained below:

#### Part 0 
Modules are imported and downloaded to run the code smoothly.

#### Part 1 - Load and Preprocess Data
The dataset is cleaned and pre-processed in this part, in which URLs, mentions and hashtags, non-alphabetic characters are removed, text is converted to lowercase, and whitespace is normalized.

#### Part 2 - Train-Test Split
The cleaned dataset is split into an 80:20 split.

#### Part 3 - Feature Extraction
Word Embedding Techniques - TF-IDF and GloVe - are extracted and implemented to the cleaned dataset to ensure optimal model performance.

#### Part 4 - Define Models
Machine learning models that will be implemented are defined in this part. The models that are used are LightGBM, Logistic Regression, XGBoost, CNN, and DNN.

#### Part 5 - Evaluate Single Models
The defined models in Part 4 are trained and evaluated individually. 

#### Part 6 - Select Top 4 Models for Hybrids
The top 4 models (has the highest accuracy) are chosen to be combined to create hybrid models. 

#### Part 7 - Create and Evaluate Hybrid Models
The chosen models from Part 6 are used to train the dataset and evaluate the model performance. 

#### Part 8 - Visualize Results
The evaluations that are gathered are visualized to help observe the model performance visually. 

A bar graph is used to show the performance of all the single and hybrid models.

A confusion matrix is used to show the performance of the top 4 single and hybrid models only. 

#### Part 9 - Save and Print Results
The results are saved to a .csv file. The results would show the evaluation of all models used, ordered by the model performance (best to worst). 

---

## Additional Notes

Other files in the repository that are not needed to detect fake news are merely original files that are modified to create the finalized .ipynb file. 

---

## Acknowledgments

This is a Group 37's term project for DS340W Spring 2025.

Written by Nayli Mohd Haniff and Vega Japarin.
