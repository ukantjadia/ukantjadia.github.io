---
title: Smart Loan Model
summary: Machine Learning Model for classifying whether to give loan or not 
tags:
  - Classification
  - ML
date: '2023-04-18T00:00:00Z'

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
    name: Follow
    url: 'https://www.linkedin.com/in/ukantjadia' 
url_code: 'https://github.com/ukantjadia/Loan-Prediction-Application'
url_pdf: 'https://github.com/ukantjadia/Loan-Prediction-Application/blob/Main/Report/Loan-Prediction-Report.pdf'
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
<!-- ![1710054038856](image/index/1710054038856.png) -->
This model is trained on a loan dataset with parameters like monthly income, gender, marital status, self-employment status, property area, etc. This model uses all the real-life factors and parameters to detect whether a loan should be given to a person or not. It helps banking or loan departments make an informed decision.

In this project, the models used for classification are logistic regression, K-nearest neighbors classifier, support vector machine, and decision tree classifier.

In this project, the following steps were taken: data collection, data preprocessing, data splitting, model implementation, and model evaluation. A detailed description of each step is given below:

1. Data Collection: I collected the data from Kaggle and read it with the `pandas` library. I analyzed the data frame using `df.info()` and `df.describe()`.
1. Data Preprocessing: For preprocessing, I dropped the duplicate values and removed and filled the null values with their respective methods, like using the median for numerical data and the mode for objective data. For visualization, I drew some plots like line plots, countplots, and bar plots for counting the loan status employment status, and other attributes to get a brief understanding of the dataset. I also generated the categorical and numerical data separately for further splitting.
1. Data Splitting: In this state, I divided the data into 80% for training and 20% for testing.
1. Model Implementation: I created a dictionary where the keys are the model names, and the values are the model instances themselves with parameters. I applied functions like loss calculation and model evaluation to this dictionary.
Output: Finally, I saved the data in a suitable format using pandas.

![1710054240434](image/index/1710054240434.png)
![1710054254673](image/index/1710054254673.png)
![1710054299247](image/index/1710054299247.png)