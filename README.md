# Shopping — Purchase Intent Prediction

An AI system that predicts whether an online shopping user will complete a purchase, using a **k-nearest neighbor classifier** (k = 1).  
This project is part of **CS50’s Introduction to Artificial Intelligence with Python**.

---

## 📦 Description

When browsing an online shopping site, most users never complete a purchase. Predicting purchasing intent can help websites customize the user experience (e.g., offering discounts or adapting content).

In this project, you will:

- Load and preprocess a dataset of ~12,000 user sessions.
- Train a **1-nearest-neighbor classifier** using scikit-learn.
- Measure performance using **sensitivity** (true positive rate) and **specificity** (true negative rate).

Example output:

```bash
python shopping.py shopping.csv 
Correct: 4088 
Incorrect: 844 
True Positive Rate: 41.02% 
True Negative Rate: 90.55%
```

---

## 🗂 Dataset

The dataset `shopping.csv` contains one row per user session and includes:

- Page visit counts and durations
- Metrics from Google Analytics (BounceRates, ExitRates, PageValues)
- Visitor metadata (browser, OS, region, visitor type, month…)
- Whether the session occurred on a weekend
- **Revenue**: whether the user completed a purchase (**label**)

The classifier must use all the other columns as **evidence** to predict _Revenue_.

---

## ▶️ Usage

Run the program with:

`python shopping.py shopping.csv`

The script will:

1. Load and preprocess the dataset
2. Train a nearest-neighbor model
3. Make predictions on a test set
4. Print accuracy, sensitivity, and specificity

---
## 📚 Acknowledgements

Dataset from:  
Sakar, C.O., Polat, S.O., Katircioglu, M. et al. _Neural Comput & Applic_ (2018).

---

Si tu veux, je peux aussi générer un **template de code complet** pour `shopping.py` conforme aux exigences CS50AI.