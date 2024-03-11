---
title: Food Image Classification
summary: A project with MLOps approach - Classifying between food and non-food image 
tags:
  - Image Processing
  - MLOps
  - Docker
  - Classification
date: '2024-01-01T00:00:00Z'

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

This project tackles the challenge of applying computer vision to emphasize accurate food image classification. It compares Convolutional Neural Networks (CNN) with Traditional Machine Learning Models, leveraging CNN's feature-rich capabilities and traditional models' transparency and computational efficiency. This dual approach enhances food image classification's precision and efficiency, impacting quality assessment, dietary analysis, and food inventory management


Used the 5K image dataset for classifying the food images and non-food images, Trained the neural network on the images for classification, and developed the model with streamlit application and achieved 80% accuracy.
The dataset is taken from [https://mmspg.epfl.ch/food-image-datasets](https://mmspg.epfl.ch/food-image-datasets) and the name of the data set is 5K.

Dataset description:
-. This dataset contains 2500 food and 2500 non-food images, for the task of food/non-food classification in our paper “Food/Non-food Image Classification and Food Categorization using Pre-Trained GoogLeNet Model”. The whole dataset is divided into three parts: training, validation and evaluation. The naming convention is as follows:
-. {ClassID}_{ImageID}.jpg
-. ClassID: 0 or 1; 0 means non-food and 1 means food.
-. ImageID: ID of the image within the class
![1710055555752](image/index/1710055555752.png)