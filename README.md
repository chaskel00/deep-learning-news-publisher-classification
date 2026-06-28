# Deep Learning News Publisher Classification

## Overview

This project was completed for my Deep Learning course at Indiana University Indianapolis.

The goal was to see whether a model could predict which news publisher wrote an article using only the headline text. The project focused on multi-class text classification across ten major news publishers.

The main question we wanted to answer was:

Can deep learning models outperform simpler text-based models when classifying news publishers from headline text?

Our original expectation was that models like CNNs and LSTMs would perform better because they can use sequence and word-order information. What we found was more interesting: the simpler Bag-of-Words / Feed-Forward model performed about as well as, or better than, the deeper models.

---

## Dataset

The dataset originally contained about 4.5 million headlines from 2007–2022. After cleaning, the dataset had about 2.1 million unique headlines.

The dataset included headlines from:

* New York Times
* CNN
* FOX
* The Guardian
* Washington Post
* BBC
* Daily Mail
* USA Today
* CNBC
* New York Post

We removed duplicate URLs, duplicate headlines, non-headline entries like “Video” and “Comments,” and other noisy text before training the models.

---

## Models Compared

The project compared several text classification approaches:

* TF-IDF + Logistic Regression baseline
* Bag-of-Words / TF-IDF Feed-Forward Neural Network
* LSTM model
* 1D CNN model

The Feed-Forward Network ended up being the strongest overall model, reaching around 57–59% accuracy. The LSTM reached around 58%, and the CNN reached around 55%.

---

## What We Found

The biggest takeaway was that deep learning did not clearly outperform the simpler text model.

A few main findings:

* Short headlines did not provide enough context for CNNs and LSTMs to show a big advantage.
* Daily Mail was much easier to classify because its headlines were much longer than the other publishers.
* Many outlets used similar wording for politics and breaking news, which caused common misclassifications.
* Headline length had a major impact on accuracy.
* More context, like lead paragraphs or full articles, would probably improve deep learning performance.

---

## My Role

My main role was helping organize the project, shape the final presentation, and communicate the results clearly. I also worked with the group on interpreting the model results and explaining why the simpler Bag-of-Words approach performed better than expected.

I am including this project because it shows my experience with text classification, model comparison, evaluation, and communicating machine learning results clearly.

---

## Repository Contents

* **Headlines_FF_NETWORK_MODEL.ipynb** – Feed-Forward Network notebook for publisher classification.
* **report/Predicting_News_Publishers_Report.pdf** – Final written report.
* **presentation/Predicting_News_Publishers_Presentation.pdf** – Final project presentation.
* **data/README.md** – Notes about the dataset source and why the full dataset is not uploaded.

---

## Skills Demonstrated

* Python
* Text preprocessing
* TF-IDF
* Bag-of-Words
* Neural networks
* Multi-class classification
* Model evaluation
* Error analysis
* Feature interpretation
* Data cleaning
* Machine learning communication

---

## Relevance to INFO-H 501

This project connects directly to several introductory data science outcomes, including data cleaning, classification, supervised learning, model evaluation, testing hypotheses, and analyzing results from a real dataset.
