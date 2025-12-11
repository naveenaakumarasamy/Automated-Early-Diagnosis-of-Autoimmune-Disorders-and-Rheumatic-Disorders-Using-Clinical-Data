# 🩺 Rheumatic Disease Prediction – End‑to‑End Machine Learning Pipeline

## 📘 Project Overview
This repository presents a **comprehensive machine learning pipeline** for the early prediction of **Rheumatic and Autoimmune Disorders** using structured clinical data. The workflow includes complete data preprocessing, feature engineering, imbalance handling, outlier detection, robust scaling, training of multiple classification models, model stacking, SHAP‑based explainability, and an interactive **Gradio web application** for real‑time prediction. The project ensures both performance and interpretability, making it suitable for research as well as preliminary clinical decision support.

---

## 🔍 Key Components of the Pipeline
### **1️⃣ Data Preprocessing & Feature Engineering**
- Missing value imputation
- Handling categorical features using Label Encoding
- Outlier removal using IQR
- Robust Scaling to minimize the influence of skewed distributions
- Class imbalance correction using **SMOTE**

### **2️⃣ Model Development**
The project evaluates multiple models:
- Logistic Regression (baseline model)
- Random Forest Classifier
- XGBoost Classifier
- Gradient Boosting Classifier
- KNN, SVM, Naïve Bayes
- **Final Stacking Ensemble Classifier** (meta‑learner: Logistic Regression)

All models are trained, evaluated, and compared based on accuracy, precision, recall, F1‑score, and AUC.

### **3️⃣ Explainability using SHAP**
- Generates SHAP Summary Plot
- Feature importance ranking
- Patient‑level interpretability for clinical usage

### **4️⃣ Deployment with Gradio UI**
A fully interactive **Gradio interface** is included for real‑time prediction. Users enter clinical parameters, and the model predicts whether the condition is **Rheumatic / Autoimmune Disorder positive or negative**, with probability scores.

---

## 📊 Evaluation & Visualizations
This project produces detailed performance insights:
- Confusion Matrix for each model
- Heatmap visualization of prediction errors
- ROC and AUC analysis
- SHAP summary charts

The final stacking model achieves **high accuracy and improved generalization** compared to individual models.

---

## 📂 Project Structure
```
📁 Rheumatic-Disease-Prediction
│
├── data/                      # Dataset (excluded for privacy)
├── models/                    # Saved trained models
├── shap_outputs/              # SHAP plots and summary files
├── app/                       # Gradio application script
├── rheumatic_pipeline.py      # Complete ML pipeline code (final version)
├── requirements.txt           # Project dependencies
└── README.md                  # Project documentation
```

---

## ⚙️ Running the Project
### **1️⃣ Clone the repository**
```bash
git clone https://github.com/your-username/rheumatic-disease-prediction.git
cd rheumatic-disease-prediction
```

### **2️⃣ Install dependencies**
```bash
pip install -r requirements.txt
```

### **3️⃣ Execute the ML Pipeline**
```bash
python rheumatic_pipeline.py
```

### **4️⃣ Launch the Gradio Application**
```bash
python app/gradio_app.py
```

---

## 📈 Results Summary
- Stacking Ensemble achieved the best predictive performance
- Gradient Boosting and Random Forest performed strongly on balanced datasets
- SHAP analysis confirms medically relevant feature contributions
- Robust preprocessing significantly improved model stability
- Gradio UI provides accessible, real‑time prediction interaction

---

## 🔮 Future Enhancements
- Integration of CNN‑LSTM models for transcriptomic data
- Deployment on cloud platforms (AWS, Azure, HuggingFace)
- Inclusion of additional biomarkers and clinical parameters
- API development for hospital EMR integration
- Mobile‑responsive UI for clinical use

---

## 🤝 Contribution Guidelines
Contributions, suggestions, and issue reports are welcome. Please open a pull request or raise an issue to discuss modifications.

---

## 📄 License
This project is licensed under the **MIT License**.

---

### ⭐ If you found this project helpful, please consider starring the repository!
