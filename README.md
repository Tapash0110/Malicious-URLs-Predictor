# 🛡️ Malicious URL Detection using Machine Learning

This project focuses on building a machine learning model to detect **malicious URLs** and classify them into two categories: `safe` and `spam`. It was trained on a labeled dataset with four original classes, which were re-labeled into binary form for simplified classification.

---

## 📂 Dataset

- The dataset originally contained **4 classes**:
  - `benign` (renamed to `ham`)
  - `phishing`, `malware`, `defacement` (all merged into `spam`)

- Final labels:
  - `ham` (label: 0)
  - `spam` (label: 1)

### Features Used:
- URL length
- Count of special characters (`.`, `/`, `@`, etc.)
- Presence of keywords (e.g., `login`, `bank`, `secure`)
- And other handcrafted features

---

## 📊 Model Performance

Three machine learning models were evaluated:

| Model                | Accuracy |
|---------------------|----------|
| Random Forest        | 93.75%   |
| XGBoost              | 92.13%   |
| K-Nearest Neighbors  | 91.88%   |

🔹 **Random Forest** was selected as the final model due to its highest accuracy.
