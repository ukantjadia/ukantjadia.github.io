---
title: Smart Loan Model
summary: Machine Learning Model for classify whether to give loan or not 
tags:
  - Classification
date: '2023-04-18T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

draft: true

image:
  # caption: Photo by raw pixel on Unsplash
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ukantjadia
url_code: 'https://github.com/ukantjadia/Loan-Prediction-Application'
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



This model is trained on a loan dataset with parameters like monthly income, gender, married, self-dependent, property_area, etc. This model uses all the real-life factors and parameters to detect whether a loan should be given to the person or not. It helps banking or loan departments make an informed decision.

This project the models for the classification which I used are logistic regression, K neighbors classifier support vector machine and Decision Tree Classifier.


In In this project these steps which I data collection data preprocessing data splitting model implementation and model evaluation A detailed description of each state is given below

1. Data collection I collected the data from kaggle and read the with  `pandas` library and analyze the data frame `df.info()` and `df.describe()`
2. Data Preprocessing: For preprocessing I drop the duplicate values and remove the and fill the null values with the their respective methods like for numerical data using the median and for objective data use mode the for visualization i drawn some plots line countplot,barplotfor counting the status and their employment status and other attributes to get a brief understanding of the data set And also also generate the categorical and the numerical data separately for further splitting
