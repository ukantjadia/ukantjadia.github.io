---
title: Heart Disease Classification with Electrocardiogram
summary: Classifying ECG data into 5 super-classes 
tags:
  - Research Paper
  - ECG
  - Classification
date: '2024-02-08T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

draft: false

image:
  # caption: Photo by raw pixel on Unsplash
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ukantjadia
  - icon: linkedin
    icon_pack: fab
    name: Connect
    url: 'https://www.linkedin.com/in/ukantjadia' 
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
Classification of 5 major types of disease/disorder from ECG dataset of PTB-XL ECG dataset(21K+ sample from 18K+ patients). the dataset for this project is taken from the official website of [physionet.org](https://physionet.org/content/ptb-xl/1.0.3/) and the name of the dataset is **PTB-XL**, a large publicly available electrocardiography dataset**.

The aim is to provide insights into the effectiveness of traditional and modern algorithms in ECG-based heart disease classification, with the potential to contribute to the improvement of diagnostic tools in the healthcare industry.

Traditional algorithms such as Support Vector Machines, Decision Trees, and Logistic Regression, alongside advanced methodologies such as Multi-Layer Perceptron and Convolutional Neural Networks.

The scope of the project includes:

- Exploring PTB-XL dataset Published: Nov. 9, 2022. Version: 1.0.3
- Preprocessing the ECG data `wfdb` and other libraries.
- Implementing traditional algorithms and advanced algorithm
- Analyzing the performance of each algorithm in terms of AUC, accuracy, precision, recall, and F1-score.
- Comparing the results to understand the strengths and weaknesses of each algorithm in classifying heart disease from the ECG dataset.

#### Images

- The dataset comprises 21837 clinical 12-lead ECG records of 10 seconds in length from 18885 patients.
For the diagnostic labels, it provides a hierarchical organization in terms of 5 coarse superclasses and 24 sub-classes for the diagnostic labels
![1710042174672](image/index/1710042174672.png)

- Columns provided in the metadata table ptbxl_database.csv. Each ECG is identified by a unique ID (ecg_id) and comes with several ECG statements (scp_codes) that can be used to train a multi-label classifier that can be evaluated based on the proposed fold assignments (strat_fold).

![1710042188040](image/index/1710042188040.png)

- Demographic overview of patients in PTB-XL.

![alt text](image/index/image.png)