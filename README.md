<div align="center">
  <h1>🤖 Machine Learning Fundamentals</h1>
  <p>
    <strong>Hands-on implementations of classical Machine Learning algorithms</strong><br>
    From concept learning and version spaces to decision tree classification
  </p>
  <p>
    <img src="https://img.shields.io/badge/Python-3.6%2B-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python">
    <img src="https://img.shields.io/badge/scikit--learn-0.19%2B-orange?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="scikit-learn">
    <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter">
    <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge" alt="Status">
    <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
  </p>
</div>

---

## 📖 About This Repository

This repository contains structured implementations of foundational Machine Learning algorithms as part of an academic lab series. Each lab is designed to build a concrete understanding of core ML concepts — from hypothesis space search to supervised classification — through practical Python code.

**Progression path:**

```
Concept Learning → Version Space Search → Decision Tree Classification
```

---

## 🎯 Aim

To implement and analyze classical Machine Learning algorithms from scratch, developing both theoretical understanding and practical coding skills in supervised concept learning and classification.

---

## 📌 Objectives

- Implement the **Find-S algorithm** to identify the most specific hypothesis consistent with positive training data
- Apply the **Candidate Elimination algorithm** to compute and narrow the version space using both positive and negative examples
- Build a **Decision Tree Classifier** using `scikit-learn` and evaluate it on a real-world categorical dataset
- Understand the role of hypothesis generalization and specialization in concept learning
- Gain hands-on experience with data preprocessing, label encoding, and model inference

---
## 🧪 Labs Overview

### Lab 1 — Find-S Algorithm (`LAB1.py`)

The Find-S algorithm is one of the simplest concept learning methods. It searches the hypothesis space from the most specific to more general hypotheses, retaining only those consistent with positive examples.

**Key Concepts:** Hypothesis space, positive example filtering, attribute generalization

---

### Lab 2 — Candidate Elimination Algorithm (`LAB2.py`)

The Candidate Elimination algorithm maintains a version space — bounded by the most specific (`S`) and most general (`G`) hypotheses — and updates both boundaries as training examples are processed.

**Key Concepts:** Version space, S and G boundary updates, positive and negative example handling

---

### Lab 3 — Decision Tree Classifier (`LAB_3_Alt.ipynb`)

A supervised classification pipeline built on the classic **Play Tennis** dataset using `scikit-learn`. Covers the full ML workflow from categorical data encoding to model training and prediction.

**Key Concepts:** Label encoding, CART decision tree, model inference, inverse transformation

| Feature     | Values                   |
|-------------|--------------------------|
| Outlook     | Sunny, Overcast, Rainy   |
| Temperature | Hot, Mild, Cool          |
| Humidity    | High, Normal             |
| Windy       | True, False              |
| PlayTennis  | Yes, No *(target)*       |

---

## ✅ Expected Outcome & Observations

| Lab | Expected Outcome |
|-----|-----------------|
| Lab 1 — Find-S | The algorithm outputs the maximally specific hypothesis consistent with all positive training examples, with `?` wildcards representing generalized attributes. |
| Lab 2 — Candidate Elimination | The final `S` and `G` boundaries converge to define a version space that is consistent with all training examples, correctly handling both positive and negative cases. |
| Lab 3 — Decision Tree | The trained classifier correctly predicts the target class (PlayTennis: Yes/No) for unseen inputs based on learned decision boundaries across the four features. |

**General Observations:**
- Find-S ignores negative examples entirely, making it sensitive to noisy data
- Candidate Elimination provides a complete picture of all consistent hypotheses but is computationally expensive for large feature spaces
- Decision Trees handle categorical data effectively but may overfit without pruning or depth constraints

---

## 🚀 Getting Started

### Prerequisites

- Python 3.6+
- Basic familiarity with Machine Learning concepts

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/machine-learning-fundamentals.git

# Install required packages
pip install numpy pandas scikit-learn jupyter
```

### Run Lab 1 & Lab 2

```bash
python LAB1.py
python LAB2.py
```

### Run Lab 3

```bash
jupyter notebook LAB_3_Alt.ipynb
```

> **Note:** Ensure `trainingdata.csv` and `tennisdata.csv` are present in the working directory before execution.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.6+ | Core language |
| NumPy | Numerical computation |
| pandas | Data manipulation and analysis |
| scikit-learn | ML model training and preprocessing |
| Jupyter Notebook | Interactive development and visualization |

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for improvements, bug fixes, or additional algorithm implementations.

---

## 📧 Contact

For questions or suggestions, please open an issue in the repository or reach out via GitHub.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">
  <p>Made with 💡 curiosity and ☕ coffee</p>
</div>
