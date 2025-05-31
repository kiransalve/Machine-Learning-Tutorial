Normalization is a feature scaling technique that rescales data to a fixed range — typically between 0 and 1

Min Max scaling is most used technique

# 🚗 ML Problem: Predicting Car Insurance Risk

## 🧠 Goal:

Predict the **risk level** (High / Medium / Low) for car insurance applicants based on:

| Feature          | Unit  | Range  |
| ---------------- | ----- | ------ |
| Age of Driver    | Years | 18–80  |
| Annual Income    | ₹     | 1L–50L |
| No. of Accidents | Count | 0–10   |

Example dataset:

| Age | Income (₹) | Accidents | Risk   |
| --- | ---------- | --------- | ------ |
| 22  | 3,00,000   | 2         | High   |
| 45  | 12,00,000  | 0         | Low    |
| 30  | 5,00,000   | 1         | Medium |

---

## ⚠️ Problem:

The features have **different scales**:

* Income is in **lakhs**
* Age is in **years**
* Accidents are in **single digits**

ML models like KNN, Logistic Regression, Neural Networks, etc., will get biased toward larger numbers (like income), leading to **poor learning**.

---

## ✅ Solution: Normalize All Features

Using **Min-Max Normalization**:

```
X_normalized = (X - min) / (max - min)
```

Assuming:

* Age: 18–80
* Income: ₹1L–₹50L
* Accidents: 0–10

After normalization:

| Age (norm) | Income (norm) | Accidents (norm) | Risk   |
| ---------- | ------------- | ---------------- | ------ |
| 0.06       | 0.04          | 0.20             | High   |
| 0.43       | 0.22          | 0.00             | Low    |
| 0.19       | 0.08          | 0.10             | Medium |

Now all features are on the **same scale (0–1)**, so ML models can learn fairly.

---

## 🤖 ML Algorithms that Need Normalization

* K-Nearest Neighbors (KNN)
* Logistic Regression
* Neural Networks
* Support Vector Machines (SVM)
* K-Means Clustering

### Algorithms that Don't:

* Decision Trees
* Random Forest
* XGBoost

---

## 🧠 Analogy:

> Comparing Age (years), Income (₹), and Accidents (count) without normalization is like comparing **apples, oranges, and bananas**.
>
> Normalization turns them into **percentage of their range**, so models compare fairly.
