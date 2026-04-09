# Satellite-land-Use-Image-Classifier-using-SVM-and-HOG
# 🌍 Satellite Land Use Image Classifier using SVM

## 📌 Overview

This project focuses on classifying satellite image patches into different land-use categories using **Machine Learning techniques**. The system uses **Histogram of Oriented Gradients (HOG)** for feature extraction and **Support Vector Machine (SVM)** for classification.

The model is trained to classify images into six categories:

* Agricultural
* Airport
* Beach
* Forest
* Port
* Urban

---

## 🎯 Objectives

* To preprocess satellite images for classification
* To extract meaningful features using HOG
* To implement Linear and RBF Kernel SVM models
* To compare model performance
* To optimize accuracy using hyperparameter tuning

---

## 🧠 Methodology

### 🔹 1. Data Preprocessing

* Load images from UC Merced dataset
* Resize images to 64×64
* Convert images to grayscale

### 🔹 2. Feature Extraction

* Extract HOG features from images
* Convert images into numerical feature vectors

### 🔹 3. Feature Scaling

* Apply Z-score normalization using StandardScaler

### 🔹 4. Model Training

* Train **Linear SVM (baseline)**
* Train **RBF Kernel SVM**

### 🔹 5. Hyperparameter Tuning

* Use GridSearchCV to optimize:

  * C (regularization parameter)
  * gamma (kernel parameter)

### 🔹 6. Evaluation

* Accuracy
* Confusion Matrix
* Precision, Recall, F1-score
* AUC score

---

## 📊 Results

| Model      | Accuracy |
| ---------- | -------- |
| Linear SVM | ~75–85%  |
| RBF SVM    | ~85–95%  |

👉 RBF Kernel SVM performs better due to its ability to handle non-linear data.

---

## 📈 Visualizations

* Sample image visualization
* HOG feature visualization
* Accuracy comparison graph
* Class-wise F1-score graph
* Prediction results

---

## ⚙️ Technologies Used

* Python
* OpenCV
* NumPy
* Scikit-learn
* Matplotlib
* Scikit-image

---

## 📂 Project Structure

```bash
Satellite-LandUse-Classifier/
│
├── dataset/
│   ├── agricultural/
│   ├── airplane/
│   ├── beach/
│   ├── forest/
│   ├── harbor/
│   ├── dense residential/
│
├── src/
│   ├── data_loading.py
│   ├── feature_extraction.py
│   ├── model_training.py
│   ├── evaluation.py
│
├── notebooks/
│   └── project.ipynb
│
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/Satellite-LandUse-Classifier.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the project:

```bash
python main.py
```

---

## 🚀 Future Scope

* Implement Deep Learning (CNN)
* Increase number of classes
* Deploy as web application
* Use real-time satellite data

---

## 🙌 Acknowledgement

This project was developed as part of academic work using the UC Merced Land Use Dataset and open-source machine learning libraries.

---

## ⭐ Conclusion

This project demonstrates that combining **HOG feature extraction with SVM classification** provides an efficient and accurate solution for satellite image classification. The use of the **RBF kernel** significantly improves performance for non-linear data.

---
