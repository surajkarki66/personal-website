---
title: "Near-Earth Object Hazard Prediction"
excerpt: "A machine learning classifier that predicts whether a Near-Earth Object is potentially hazardous, with explainable predictions."
collection: portfolio
permalink: /portfolio/near-earth-objects-danger-risk-prediction/
header:
  teaser: portfolio/thumbs/neo.jpg
---

![Near-Earth Object Hazard Prediction](/images/portfolio/neo.png)

This project predicts whether a Near-Earth Object (NEO) is potentially hazardous using machine learning. Trained on NEO observations recorded between 1910 and 2024, the model classifies objects as hazardous or non-hazardous, supporting NEO risk assessment.

**Highlights**

* Full workflow: data cleaning, exploratory data analysis, handling class imbalance, model training, and evaluation, with PyCaret and Scikit-learn.
* A Random Forest classifier achieved the best accuracy among the models tested.
* Explainable predictions with LIME, highlighting key features such as absolute magnitude, estimated diameter, relative velocity, and miss distance.
* Model serialized with Skops and served through an interactive Streamlit app (also runnable with Docker).

**Tech stack:** Python · Pandas · Scikit-learn · PyCaret · LIME · Skops · Streamlit

[Source code](https://github.com/surajkarki66/Near_Earth_Objects_Danger_Risk_Prediction)
