# Parkinsons-Disease-Prediction-using-ML

Parkinson's Disease Prediction using Machine Learning
🚀 Project Overview
This project leverages the power of Machine Learning (ML) to predict the presence of Parkinson's Disease in individuals based on voice-based features. Using a dataset of voice recordings, various ML algorithms have been employed to classify patients as either having Parkinson’s Disease or being healthy, aiming to assist in early diagnosis and monitoring.

🧠 Problem Statement
Parkinson’s Disease is a neurodegenerative disorder that affects motor control, often going unnoticed in the early stages. Early diagnosis can dramatically improve patient care, but traditional methods are invasive, costly, and sometimes unreliable. The goal of this project is to create a predictive model based on voice features (such as jitter, shimmer, and harmonics-to-noise ratio) to aid in early diagnosis and help clinicians detect symptoms sooner.

🔍 Dataset
The dataset used in this project contains voice recordings from individuals with and without Parkinson's Disease, including features extracted from the recordings, such as:

Jitter: Variation in fundamental frequency

Shimmer: Variation in amplitude

Harmonics-to-Noise Ratio: Noise level in voice

Mel-Frequency Cepstral Coefficients (MFCC): Features used in speech and audio analysis

The dataset is publicly available on UCI Machine Learning Repository.

⚙️ Key Features & Methodology
Data Preprocessing

Handling missing values

Normalization and standardization of features

Feature Engineering

Selection of relevant features from voice data

Dimensionality reduction using PCA (Principal Component Analysis)

Machine Learning Models

Random Forest

Support Vector Machine (SVM)

K-Nearest Neighbors (KNN)

Logistic Regression

Model Evaluation

Cross-validation and hyperparameter tuning using GridSearchCV

Performance metrics: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

💡 Project Insights
Early Diagnosis: The model is capable of predicting the likelihood of Parkinson’s Disease with significant accuracy, making it a potentially useful tool for healthcare practitioners.

Voice-Based Prediction: By using speech features rather than traditional methods like imaging, this system provides a non-invasive, cost-effective solution for preliminary diagnosis.

Model Comparison: Different algorithms were tested, with Random Forest emerging as the best performer in terms of accuracy and precision.

📊 Results
Random Forest Model: Achieved an accuracy of 98%, with an F1-Score of 0.97.

SVM Model: Achieved an accuracy of 95%, with a slightly lower recall rate.

🛠️ Installation & Usage
To get started with the Parkinson’s Disease Prediction project, follow the steps below:

Prerequisites
Ensure you have Python (>= 3.7) and the following libraries installed:

pandas

numpy

scikit-learn

matplotlib

seaborn

pickle (for saving models)

1. Clone the repository
bash
Copy
Edit
git clone https://github.com/yourusername/Parkinsons-Disease-Prediction-using-ML.git
cd Parkinsons-Disease-Prediction-using-ML
2. Install required libraries
bash
Copy
Edit
pip install -r requirements.txt
3. Run the model
bash
Copy
Edit
python parkinsons_predictor.py
4. Example usage
python
Copy
Edit
from model import predict_parkinsons

# Example input: [jitter, shimmer, ...]
features = [0.005, 0.02, 12.4, 0.15, 0.97, ...]
result = predict_parkinsons(features)

if result == 1:
    print("Prediction: Parkinson's Disease")
else:
    print("Prediction: Healthy")
📈 Visualizations & Insights
Below are a few key visualizations that give insights into the dataset and model performance:

Feature Correlation Heatmap

Model Accuracy and Precision Comparison

Confusion Matrix

These plots are generated using Matplotlib and Seaborn to help visualize the results and ensure transparent and understandable model evaluation.

🤝 Contributing
Feel free to fork this repository, contribute by improving the model, or suggesting optimizations. Contributions can include:

Testing additional ML algorithms

Improving feature engineering

Providing more datasets

Creating deployment scripts for real-time prediction

To contribute, please fork the repository, create a new branch, and submit a pull request.

📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

🧑‍💻 Acknowledgments
UCI Machine Learning Repository for the dataset.

Scikit-learn for machine learning tools and algorithms.

Matplotlib & Seaborn for data visualization.
