# Machine-Learning-Fundamentals
A repository to help the TVET Curriculum educators to explore some practical concepts in machine learning based on how RTB curriculum structured, This repo will be updated with new Learning outcomes soon, stay checking updates.
# 🧼 1. Data Preprocessing Techniques with Synthetic Data

This Jupyter notebook demonstrates key data preprocessing techniques using a small synthetic dataset. It is designed as a learning tool for Teachers / students and beginners in Machine Learning.

## ✨ Covered Topics
you are welcome to contribute to this repo if you are passionate to help others especially educators
---

## ✨ Covered Topics

- Handling missing data
- Feature encoding:
  - Label Encoding
  - Binary Encoding
  - Target Encoding (with and without smoothing)
- Feature scaling (MinMax Scaler, Standard Scaler)
- Date/time feature extraction and transformation and Cycling encoder( SINUS AND COSINE representation to detect the close betwen DECEMBER(12) AND JANUARY(1))
- Correlation analysis And interpretation
- Normality testing (e.g., Kolmogorov–Smirnov test)
- Dropping irrelevant features

---

## 📁 Included Files

- `data cleaning with syntetic data.ipynb` – Main notebook with all examples and explanations.
- `Data.csv` – Small dataset created for teaching purposes.

---
# 🧼 2. CLASSIFICATION MODEL
AS We learn by doing real project, This Bank note classification project focuses on classifying banknotes as FAKE or REAL using machine learning algorithms. It uses a dataset containing features extracted from images of banknotes, including statistical properties like variance, skewness, kurtosis, and entropy.

🧠 Models Used:
- K-Nearest Neighbor (KNN)
- Logistic Regression

## ✨ Covered Topics

- Choosing the best value of K to be used in KNN using K-fold Cross validation
- training KNN MODEL
- train Logistic Regression Model
- Evaluation Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1 score
- Confusion Matrix

## 📁 Included Files

- `BANK NOTE CLASSIFICATION` – Main notebook with all examples and explanations.
- `BankNote_Authentication.xls` – Small dataset used from Kaggle platform.

# 🌺 3. FLOWER IMAGE CLASSIFICATION MODEL USING CNN
<img width="881" alt="image" src="https://github.com/user-attachments/assets/5a12463c-46ad-426c-9c2e-7d2780f5b401" />

As we continue learning through real projects, this Flower Classification project uses a Convolutional Neural Network (CNN) to classify images into five flower types:

### 🌼 Lilly 🌸 Lotus 🌺 Orchid 🌻 Sunflower 🌷 Tulip

## 🧠 Model Used
🧱 Custom CNN with 3 Convolutional Layers

### ✨ Covered Topics
🖼️ Image classification using CNN

🛠️ Building & training a 3-layer CNN from scratch

📊 Visualizing training accuracy and loss

📈 Evaluation Metrics:

✅ Accuracy

🎯 Precision

🔁 Recall

🧮 F1 Score

🔍 Confusion Matrix analysis
# what used in development ?
1. 📁 Dataset Handling & Preprocessing
split-folders:
Used to automatically split the dataset (flower_images) into training and validation sets while preserving class folders.

python
Copy
Edit
splitfolders.ratio("flower_images", output="flowers_split", seed=1337, ratio=(.8, .2))
ImageDataGenerator (tensorflow.keras.preprocessing.image)
For real-time data augmentation and loading of images during training.

PIL (Python Imaging Library)
Used internally by Keras for image processing (e.g., resizing, loading images).

2. 🧰 Model Development
TensorFlow / Keras:
Main deep learning library used for defining, training, and saving the Convolutional Neural Network.

CNN Architecture:
Built using Keras Sequential API with layers like:

Conv2D, MaxPooling2D, Flatten, Dense, Dropout

Model Saving:

Saved using .h5 or recommended .keras format

model.save("model_name.h5") or model.save("model_name.keras")

3. 📊 Evaluation
matplotlib:
For visualizing training/validation accuracy and loss.

sklearn.metrics:
For computing the confusion matrix and evaluating model performance on the test set.

4. 🧪 Testing & Prediction
numpy:
For array manipulation when loading test images.

tensorflow.keras.preprocessing.image:
For manually loading and preprocessing a single test image using:

python
Copy
Edit
image.load_img(), image.img_to_array(), np.expand_dims(), etc.
5. 🌐 User Interface
Gradio:
Used to build a simple web interface where users can upload an image and get the predicted flower class.

Features: File Upload, Live Prediction, Easy Web UI Integration
## 📁 Included Files
CNN_FLOWER_CLASSIFICATION.ipynb – Main notebook with full model implementation
📥 Dataset (1000+ images per class):
⬇️ Download from Google Drive(https://drive.google.com/file/d/1ZuMforenbdcq3rLNa9itBawdZNqk-PCY/view?usp=sharing)


## 💻 How to Run This Notebook Locally

### 1️⃣ Prerequisites
Make sure you have **Python 3.x** and **pip** installed. You can install Python from the [official website](https://www.python.org/downloads/).

### 2️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

pandas
numpy
scikit-learn
category_encoders
matplotlib
seaborn
scipy
Let me know if you'd like a version for publishing on **Kaggle**, **Google Colab**, or a **custom webpage** too!
```
## 🧑‍🏫 Author

**NIYONSHUTI Yves**  
Assistant Lecturer – Rwanda Polytechnic, Tumba College  
Founder & CEO – Mpuza Inc.  
📧 yniyonshuti@rp.ac.rw  📧 info@mpuza.com 
https://mpuza.com  https://www.linkedin.com/company/mpuza/?viewAsMember=true
📞 +250 786 397 515
CONTACT ME FOR ANY FURTHER EXPLANATION AND TECHNICAL SUPPORT
---

## 💡 Purpose

This repository serves as a teaching resource to help learners understand and practice data preprocessing techniques before moving on to real-world data science problems.

---

## 🔒 Note on Reuse

Feel free to use and share this notebook with **attribution**. The content is intended for educational purposes.

---
