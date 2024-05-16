---
title: Bloom's Taxonomy Level Detection
summary: Detecting Bloom's level of given input statement out of six levels
tags:
  - Research Paper
  - OBE
  - Classification
  - MLOps
  - NLP
date: '2023-12-13T00:00:00Z'

# Optional external URL for projects (replaces project detail page).
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
url_code: 'https://github.com/ukantjadia/Boolm-s-Level-Detection-A-MLOPS-Project/'
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


<!-- For using this project here is a Streamlit app URL(it will take some time to launch) [https://ukant.tech/Boolm-s-Level-Detection-A-MLOPS-Project/] -->

To know Bloom's Taxonomy in Detail see this pdf [This](./blooms-level.pdf)

This project aims to classify the given statement into accurate Bloom's taxonomy levels out of six levels. This is an NLP-based project. This project is built with TF-IDF vectorizer and multinomial Naive Bayes techniques. 

**Bloom's Taxonomy Levels**: Bloom’s Taxonomy is a classification system that arranges learning objectives into six hierarchical levels, each representing a different cognitive skill.

The model is trained on 1800 augmented statements. Initially, I had 100 statements for each class, so a total of 600 statements for six classes. Then, this data is augmented three times using contextual word embedding augmentation, and the model used in the augmentation is BERT-based. An example of the augmentation methodology.

 <!-- is inserted below

augmented each Text input 3 times with the following parameter with `nlpaug` library
```python
ContextualWordEmbsAug(model_path="bert-base-uncased", action="insert")
```

> before augmendatation data shape : 600,2                                  
> total 6 unique calsses 100 each                                   
> augmented data shape : 1800,2                                  
> total 6 unique classes 300 each                                   -->

This project follows MLOps techniques well. I have divided this project into 6 different pipelines for easy implementation and scalability. I created a class in the pipeline for each class using different entities and components. In generating a configuration file from the user input in the YAML format. 

In the end, I created a Docker image so it can be used by the Higher Education Institute(HEIs) for those who are using the OBE(Object Based Education) new curriculum technique. It just reduced the manual process of identifying each question and its root taxonomy level.

![1710044827297](image/index/1710044827297.png)


![1710044894646](image/index/1710044894646.png)

![1710044907287](image/index/1710044907287.png)
