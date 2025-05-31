# Feature Engineering

Feature engineering is the process of creating or modifying input data (features) to help a machine learning model learn better and make more accurate predictions.

---

## Simple Example:

If you have a **date** column, you can create new features like **day**, **month**, or **weekday** — this helps the model understand patterns better.

---

## Why it’s important:

- **Good features = Better model performance**  
- **Poor features = Poor results, even with advanced algorithms**

---

## 1. Feature Transformation

### Missing Values Imputation:

- Our data has missing or empty (Null) values.
- ML algorithms **do not accept data with missing values**.
- So, we have to **fill** or **remove** them.
- If missing values are few, we can **remove** those rows.
- But if many values are missing, we have to **fill** (impute) them.

---

### Handling Categorical Features

We convert categorical data into numerical format.

![handling categories](https://github.com/user-attachments/assets/48941b7c-494b-4437-803b-c41f5491ba29)

---

### Outlier Detection

Outlier detection means finding data points that are very different from the rest — values that are too high or too low compared to others.

#### Why Detect Outliers?

- They can **skew averages or results**.
- They might show **errors in data** (like a typo ₹999999 instead of ₹999).
- Or they might reveal something important — like **fraud** or **unusual behavior**.

---

### Feature Scaling

**"Normalize to Optimize"**

Feature scaling means adjusting the values of your data so that all features are on a similar scale (range).

This helps machine learning models learn better and faster, especially models that rely on distance or gradient-based optimization.

#### Why is Feature Scaling Important?

Some algorithms are sensitive to the scale of features.

If one column has values from 0–1000 and another from 0–1, the model might give more importance to the bigger numbers — even if they aren’t more important.

| Needs Scaling         | Doesn’t Need Scaling |
| --------------------- | -------------------- |
| ✅ KNN                 | ❌ Decision Trees     |
| ✅ SVM                 | ❌ Random Forest      |
| ✅ Logistic Regression | ❌ XGBoost            |
| ✅ Neural Networks     | ❌ Naive Bayes        |

---

## 2. Feature Construction

Feature construction is the process of creating new features from existing data to help a machine learning model understand the problem better.

| Original Features             | New Constructed Feature            |
| ----------------------------- | ---------------------------------- |
| `Price` and `Quantity`        | `Total Sales = Price × Quantity`   |
| `Date`                        | `Day`, `Month`, `IsWeekend`        |
| `First Name`, `Last Name`     | `Full Name`                        |
| `Order Date`, `Delivery Date` | `Delivery Time = Delivery - Order` |
| `Height` and `Weight`         | `BMI = Weight / (Height^2)`        |

---

## 3. Feature Selection

Feature selection means choosing the most important columns (features) from your dataset and removing the useless or less useful ones.

> **Feature selection = Keep the best, drop the rest.**
