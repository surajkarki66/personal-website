---
title: "MediLeaf"
excerpt: "An Android app that identifies medicinal plants and their properties by scanning a leaf, powered by a CNN with over 95% accuracy."
collection: portfolio
permalink: /portfolio/medileaf/
header:
  teaser: portfolio/thumbs/medileaf.jpg
---

![MediLeaf](/images/portfolio/medileaf.png)

MediLeaf is an Android application that helps people identify medicinal plants and learn about their properties simply by scanning a leaf. By making plant knowledge accessible, it aims to spark curiosity about medicinal plants, support their preservation, and highlight their value as a source of income.

**Highlights**

* CNN-based leaf classifier with over 95% accuracy, with data and model versioning in DVC.
* Three-part architecture: an AI model server that predicts the plant species, a knowledge-base server for plant properties and significance, and a Flutter mobile app that brings them together.
* Backend services containerized with Docker.

**Tech stack:** TensorFlow · Scikit-learn · CNN · DVC · FastAPI · Django · PostgreSQL · Flutter · Docker

Source code: [Mobile app](https://github.com/surajkarki66/MediLeaf_Mobile) · [AI model server](https://github.com/surajkarki66/MediLeaf_AI) · [Knowledge-base server](https://github.com/surajkarki66/MediLeaf_backend)
