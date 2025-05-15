# 🧬Breast_Cancer_Model
This project utilizes the Breast Cancer Wisconsin (Diagnostic) Dataset to build a machine learning model that classifies breast tumors as malignant or benign based on various features extracted from digitized images of fine needle aspirates (FNA) of breast masses.

📌 Overview
The goal is to help early detection of breast cancer using machine learning, which can potentially assist healthcare professionals in diagnosis. The model is trained using scikit-learn's RandomForestClassifier for high performance and interpretability.

📂 Dataset
Source: UCI Machine Learning Repository
Name: Breast Cancer Wisconsin (Diagnostic) Data Set
Attributes: 30 numeric features (mean, standard error, and worst of 10 cell nucleus properties)
Target: Diagnosis (M = malignant, B = benign)

The dataset is programmatically downloaded using kagglehub:
import kagglehub
path = kagglehub.dataset_download("uciml/breast-cancer-wisconsin-data")

🛠️ Features Used
Radius, Texture, Perimeter, Area, Smoothness, Compactness, Concavity, Concave Points, Symmetry, Fractal Dimension
Each feature includes: mean, standard error, and "worst" (largest of 3 values)

🧪 Model Building
The pipeline involves:
1. Loading and preprocessing the dataset
2. Encoding labels (Malignant = 1, Benign = 0)
3. Scaling features using StandardScaler
4. Splitting the dataset into training and testing sets
5. Training a RandomForestClassifier
6. Evaluating with accuracy, confusion matrix, and classification report

🔍 Evaluation Metrics
Accuracy Score
Confusion Matrix
Classification Report (Precision, Recall, F1-score)

✅ Results
The model achieves high accuracy and provides clear classification between benign and malignant tumors. Random Forest offers feature importance analysis as well, aiding interpretability.

📦 Requirements
pandas
numpy
scikit-learn
kagglehub

📜 License
This project is open-source and free to use under the MIT License.
