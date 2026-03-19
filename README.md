# 🧠 Machine Learning From Scratch: KNN & Naive Bayes

This project implements two fundamental machine learning algorithms completely from scratch using pure Python:

* **K-Nearest Neighbors (KNN)**
* **Gaussian Naive Bayes**

The goal of this project is to deeply understand the **mathematical foundations** behind these algorithms by avoiding high-level machine learning libraries such as NumPy, pandas, or scikit-learn.

---

## 📌 Project Objectives

* Build machine learning algorithms **from first principles**
* Understand how models work **under the hood**
* Avoid abstraction and focus on **core logic and math**
* Visualize algorithm behavior using **custom SVG-based illustrations**

---

## 🚫 Constraints (What I Did NOT Use)

To stay true to the “from scratch” philosophy, I intentionally avoided:

* ❌ NumPy
* ❌ pandas
* ❌ scikit-learn
* ❌ matplotlib

Instead, I only used:

* ✅ Basic Python (lists, loops, dictionaries)
* ✅ `math` and `random` (standard library)
* ✅ Manual SVG generation for visualization

---

## 📂 Project Structure

```
ai-from-scratch-naive-bayes-knn/
│
├── notebooks/
│   └── 01_naive_bayes_knn_from_scratch.ipynb
│
└── README.md
```

---

## 📊 Dataset

The dataset is **synthetically generated in code**.

Each data point:

```
[x1, x2, label]
```

* Two features: `x1`, `x2`
* Binary classification: `0` or `1`
* Two Gaussian clusters:

  * Class 0 → lower-left region
  * Class 1 → upper-right region

This makes it easier to:

* Visualize decision behavior
* Understand how each algorithm separates classes

---

## 🤖 Algorithms Implemented

### 1. K-Nearest Neighbors (KNN)

**Core Idea:**

* Compute distance between a query point and all training points
* Select the `k` nearest neighbors
* Predict based on majority vote

**Key Concepts Learned:**

* Euclidean distance
* Local decision boundaries
* Lazy learning (no explicit training phase)

---

### 2. Gaussian Naive Bayes

**Core Idea:**
Uses Bayes' Theorem:

P(class | x) ∝ P(class) × P(x | class)

Assumes:

* Features are conditionally independent
* Each feature follows a Gaussian (normal) distribution

**Key Concepts Learned:**

* Prior probabilities
* Likelihood estimation
* Gaussian distributions (mean & variance)
* Independence assumption

---

## 🎨 Visualizations

Instead of using plotting libraries, this project uses **custom-built SVG graphics** to illustrate:

* Dataset distribution
* KNN neighbor selection and voting
* Naive Bayes probability modeling

These visuals are designed to:

* Explain *how* the algorithms work
* Improve conceptual understanding (not just performance analysis)

---

## 📈 Evaluation Metrics

Simple evaluation methods were implemented from scratch:

* **Accuracy**
* **Confusion Matrix**

This reinforces understanding of:

* Model correctness
* Classification errors

---

## 🧠 Key Takeaways

* KNN is **intuitive but computationally expensive at prediction time**
* Naive Bayes is **fast and compact but relies on strong assumptions**
* Implementing from scratch exposes:

  * Hidden complexity behind simple APIs
  * Importance of mathematical modeling
* Visualization helps bridge the gap between:

  * Code → Math → Intuition

---

## 🚀 Future Improvements

Potential next steps:

* Add feature scaling / normalization
* Support multi-class classification
* Implement weighted KNN
* Extend Naive Bayes to categorical features
* Test on more complex / overlapping datasets

---

## 💡 Why This Project Matters

Most machine learning tools abstract away the details.
This project focuses on understanding what actually happens behind the scenes.

By building everything manually, I gained a deeper understanding of:

* How models make decisions
* How data distribution affects performance
* The trade-offs between different algorithms

---

## 📎 How to Run

1. Open JupyterLab
2. Navigate to:

```
notebooks/01_naive_bayes_knn_from_scratch.ipynb
```

3. Run all cells sequentially

---

## 🏁 Final Note

This project is not about performance — it is about **understanding**.

Every line of code is written to reflect the underlying mathematics as clearly as possible.s