---
title: 'ECG-Lense: Benchmarking ML & DL Models on PTB-XL Dataset'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  # - Robert Ford

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2024-08-01T00:00:00Z'
doi: 'https://doi.org/10.1109/ETNCC63262.2024.10767459'

# Schedule page publish date (NOT publication's date).
publishDate: '2024-23-07T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *International Conference on Emerging Trends in Networks and Computer Communications*
publication_short: In ETNCC

abstract: Automated classification of electrocardiogram (ECG) signals is a useful tool for diagnosing and monitoring cardiovascular diseases. The process can be aided by the use of machine learning (ML) and deep learning (DL) techniques. This study compares three traditional machine learning algorithms (Decision Tree Classifier, Random Forest Classifier, and Logistic Regression) and three deep learning models (Simple Convolutional Neural Network (CNN), Long Short-Term Memory (LSTM), and Complex CNN (ECG-Lense)) for the precise classification of ECG signals from the PTB-XL dataset. This dataset has 12-lead ECG recordings from normal patients and patients with various cardiac conditions. The DL models were trained on raw ECG signals, allowing them to automatically extract important features. Additionally, data augmentation techniques were used to enhance model performance increase the diversity of training samples, and maintain the essential characteristics of the ECG signal data. The models were thoroughly evaluated using multiple metrics, such as precision, recall, F1-score, and ROC-AVC. The results indicate that the Complex CNN (ECG-Lense) model surpassed the other algorithms with an 80% classification accuracy and a 90% ROC-AUC. This research not only highlights the best heart ECG-based classification model but also sheds light on the strengths and limitations of the machine and deep learning methods in this area. Healthcare professionals can utilize these findings to automate ECG interpretation and enhance patient care strategies. Additionally, the comparative analysis paves the way for future research to create more advanced and specialized models for specific cardiac conditions, ultimately leading to the early detection and effective management of heart-related disorders.

# Summary. An optional shortened abstract.
summary: This study evaluates machine learning and deep learning models for classifying ECG signals from the PTB-XL dataset. It compares six models, including Random Forest, Logistic Regression, CNN, LSTM, and a complex CNN called ECG-Lense. The ECG-Lense model achieved the highest accuracy (80%) and ROC-AUC (90%) using raw signals and data augmentation. Findings support automated ECG analysis for improved diagnosis and future cardiac researchThis study evaluates machine learning and deep learning models for classifying ECG signals from the PTB-XL dataset. It compares six models, including Random Forest, Logistic Regression, CNN, LSTM, and a complex CNN called ECG-Lense. The ECG-Lense model achieved the highest accuracy (80%) and ROC-AUC (90%) using raw signals and data augmentation. Findings support automated ECG analysis for improved diagnosis and future cardiac research.

tags:
  -  Electrocardiogram(ECG)
  -  Cardiovascular Disease
  -  PTB-XL Dataset
  -  Deep Learning
  -  Machine Learning

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: 'https://github.com/ukantjadia/Major-Projectr'
url_dataset: 'https://physionet.org/content/ptb-xl/1.0.3/'
url_poster: ''
url_project: 'https://github.com/ukantjadia/vs-code-Profiles/blob/Main/content/Final%20Presentation%20Report.pdf'
url_slides: 'https://github.com/ukantjadia/vs-code-Profiles/blob/Main/content/Final%20Presentation%20Ukant%20Jadia.pdf'
url_source: 'https://github.com/ukantjadia/Major-Project'
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'ECG-Lense Model(https://github.com/ukantjadia/vs-code-Profiles/blob/Main/content/CNN-model.png)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - content/project/heart-ECG-project/index.md

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---
