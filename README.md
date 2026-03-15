# 🏥 Breast Cancer Tumor Classification using Machine Learning and Generative AI

A healthcare data science project that predicts whether a breast tumor is **malignant** 
or **benign** using machine learning, and uses Google Gemini AI to communicate the 
results in plain, clinical language.

---

## 📌 Project Overview

Early detection of breast cancer significantly improves patient survival rates. However, 
accurate tumor diagnosis typically requires specialist expertise that is not equally 
accessible across all healthcare settings. This project explores whether a machine 
learning model can reliably classify tumors based on measurable cell characteristics, 
and whether Generative AI can then present those findings in a way that is meaningful 
to a non-technical clinical audience.

The project was built entirely in Google Colab using free, open-source tools and 
a publicly available medical dataset.

---

## 🎥 Walkthrough Video

[▶️ Click here to watch the full project walkthrough](PASTE YOUR LOOM LINK HERE)

---

## ✅ Project Requirements

| Requirement | Implementation |
|---|---|
| **Data Processing** | Data quality check, class distribution analysis, and 3 targeted visualizations |
| **Machine Learning** | Random Forest Classifier trained on 30 tumor features |
| **Generative AI** | Google Gemini API used to generate a plain-English clinical summary |

---

## 📊 Model Results

| Metric | Score |
|---|---|
| Overall Accuracy | **96.49%** |
| Malignant Recall | **99%** |
| Malignant Precision | 96% |
| Benign Recall | 93% |
| Benign Precision | 98% |
| Test Set Size | 114 samples |

> In a cancer screening context, **malignant recall is the most critical metric** 
> because a false negative (missing a real cancer) is far more dangerous than a 
> false positive. The model correctly identified 70 out of 71 malignant cases in 
> the test set.

---

## 📁 Repository Contents
```
├── healthcare_capstone.ipynb        # Full project notebook (Google Colab)
├── capstone_written_responses.docx  # Written responses to all 3 assessment questions
├── ai_summary.txt                   # Gemini AI generated clinical summary output
├── diagnosis_distribution.png       # Chart: Benign vs malignant case counts
├── feature_comparison.png           # Chart: Feature distributions by diagnosis
├── correlation_heatmap.png          # Chart: Feature correlation heatmap
├── confusion_matrix.png             # Chart: Model prediction confusion matrix
├── feature_importance.png           # Chart: Top 10 most important features
└── README.md
```

---

## 🔬 Dataset

**Wisconsin Breast Cancer Dataset**
- Built into scikit-learn — no external download required
- 569 real patient samples
- 30 numerical features derived from digitized tumor cell biopsy images
- Binary classification: malignant (212 samples) vs benign (357 samples)
- Originally collected at the University of Wisconsin

---

## 🛠️ Tools and Libraries

| Tool | Purpose |
|---|---|
| Google Colab | Cloud-based notebook environment |
| Python | Primary programming language |
| Pandas | Data loading and quality checking |
| Matplotlib & Seaborn | Data visualization |
| scikit-learn | Machine learning model and evaluation |
| Google Gemini API (`google-genai`) | Generative AI clinical summary |

All tools used in this project are **free of cost**.

---

## 🧠 Key Findings

- **Worst area**, **worst concave points**, and **mean concave points** were the 
  three most important features for predicting malignancy, with importance scores 
  of 0.15, 0.14, and 0.105 respectively.
- Size and shape irregularity measurements consistently outperformed texture-based 
  features, which aligns with established medical understanding of malignant tumor 
  characteristics.
- Mean radius, mean perimeter, and mean area showed near-perfect correlation 
  (0.99 to 1.00), confirming that these features all capture the same underlying 
  characteristic: tumor size.

---

## ⚠️ Disclaimer

This project is an academic capstone submission built for educational purposes. 
The model is a decision-support demonstration only. It is **not a medical diagnostic 
tool** and must never be used as a substitute for professional clinical diagnosis. 
All medical decisions must be made by qualified healthcare professionals.

---

## 👤 Author

**Prince Kawser**  
Capstone Project — Data Analytics and AI Program  
Digital Nova Scotia  
2026
