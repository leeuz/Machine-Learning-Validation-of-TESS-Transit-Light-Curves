# Machine Learning Validation of TESS Transit Light Curves  
### Case Study: TOI-7325.01

## Overview
This project applies supervised machine learning to classify transit candidates from NASA’s Transiting Exoplanet Survey Satellite (TESS) as likely exoplanets or false positives. By extracting basic features from TESS light curves—such as transit depth, duration, average flux, and flux variability—a Random Forest model is trained to estimate the probability that a given transit signal corresponds to a real exoplanet.

As a case study, the model evaluated TOI-7325.01 and assigned it a probability of **0.73**, suggesting a strong likelihood of being a genuine exoplanet. The results demonstrate that relatively simple light curve features can provide useful early-stage guidance when validating exoplanet candidates.

This work was conducted as part of the NASA–GMU Research Scholar program and resulted in a peer-reviewed publication.

---

## Research Abstract
This paper uses machine learning to sort transit candidates from TESS into likely exoplanets or false positives. Features such as transit depth, duration, average flux, and flux variation were extracted from TESS light curves to train a Random Forest model. The model determines the probability that a candidate is an actual exoplanet, assisting in identifying which targets warrant further observation. For example, the model assigned TOI-7325.01 a probability of 0.73, suggesting a strong likelihood of being a real exoplanet. The results show that basic light curve features can provide useful early validation of exoplanet candidates. Future work could incorporate additional stellar parameters and larger datasets to improve predictive accuracy and extend the method to more TESS Objects of Interest.

---

## Dataset
- **Source:** NASA TESS Mission
- **Data Type:** Transit light curves for TESS Objects of Interest (TOIs)
- Raw light curve data is not included in this repository due to size and licensing considerations.
- Instructions for obtaining the data are provided in the `data_instructions.md` file.

---

## Feature Engineering
The following features were extracted from each light curve:
- Transit depth  
- Transit duration  
- Average flux  
- Flux variability  

These features were selected to capture key transit characteristics while remaining computationally efficient.

---

## Model
- **Algorithm:** Random Forest Classifier
- **Learning Type:** Supervised learning
- **Task:** Binary classification (exoplanet vs. false positive)
- **Output:** Probability score indicating likelihood of a true exoplanet

---

## Results
- **TOI-7325.01 predicted probability:** **0.73**
- The model demonstrates that basic photometric features can be effective for early-stage exoplanet validation.

---

## Publication
This work was co-authored with Prof. Peter Plavchan and officially published in the George Mason University Libraries – MARS Publishing Community.

**DOI:** https://doi.org/10.13021/MARS/15194

---

## Repository Structure
