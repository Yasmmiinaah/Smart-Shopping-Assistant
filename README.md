# 🛍️ Smart Multimodal Shopping Assistant

## 📌 Project Overview

The Smart Multimodal Shopping Assistant is a deep learning based recommendation and similarity system that combines both image and text understanding.

The system takes:

* A product image or short visual input
* A textual preference description

Then it predicts:

* The most similar products
* Or a numerical similarity score

This project follows a Multimodal Deep Learning approach by combining Computer Vision and Natural Language Processing.

---

# 🎯 Problem Statement

Traditional shopping systems rely only on images or only on textual search.

However:

* Images contain visual details such as shape, style, and color.
* Text descriptions contain semantic preferences and product characteristics.

Using a single modality may reduce recommendation quality.

Therefore, this project combines:

* Visual features extracted from images
* Semantic features extracted from text

The goal is to improve intelligent product matching and recommendation accuracy.

---

# 🧠 Deep Learning Architecture

## 🔹 Image Models

### 1. ResNet50

Used for extracting deep visual features from product images.

### 2. EfficientNet

Used as an alternative CNN architecture for image classification and feature extraction.

---

## 🔹 Text Models

### 3. GRU (Gated Recurrent Unit)

Processes textual product descriptions and extracts semantic representations.

### 4. LSTM (Long Short-Term Memory)

Used for sequential text understanding and feature extraction.

---

## 🔹 Fusion Model

### 5. Concatenation Model

Combines:

* Image feature vectors
* Text feature vectors

into a shared multimodal representation space.

---

## 🔹 Similarity Model

### 6. Cosine Similarity Model

Computes similarity between image and text embeddings.

Used to:

* Rank products
* Retrieve the most relevant items
* Generate recommendation results

---

# 🖼️ Workflow

1. Product image is processed using CNN models.
2. Text description is processed using GRU/LSTM.
3. Both embeddings are fused using concatenation.
4. Features are projected into a shared embedding space.
5. Cosine Similarity is calculated.
6. Results are ranked according to similarity score.

---

# 📂 Dataset

The dataset was prepared and customized specifically for the project.

Dataset contains:

* Fashion product images
* Product descriptions
* Product categories

### Classes

* bags
* outfit
* pants
* shirts
* shoes
* skirt
* watches

---

# 📊 Evaluation Metrics

The project uses multiple evaluation metrics including:

* Accuracy
* Validation Accuracy
* Loss
* Validation Loss
* Cosine Similarity Score

---

# 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* VS Code

---

# 📁 Project Structure

```text
Multimodal_Project/
│
├── Notebook1.ipynb
├── Notebook2.ipynb
├── Notebook3.ipynb
│
├── resnet50_fashion_model.keras
├── efficientnet_model.keras
├── gru_feature_extractor.keras
├── lstm_text_encoder.keras
├── fusion_model.h5
├── tokenizer.pkl
│
├── class_names.json
├── requirements.txt
├── README.md
│
└── dataset/
```

---

# 👥 Team Contributions

The project was divided into multiple deep learning tasks:

* Image Modeling
* Text Modeling
* Fusion Architecture
* Similarity Computation
* Evaluation & Testing
* Dataset Preparation

---

# 🚀 Future Improvements

Possible future enhancements include:

* Real-time recommendation system
* Video-based recommendation
* Transformer-based text encoders
* Attention mechanisms
* Larger multimodal datasets

---

# ✅ Conclusion

This project demonstrates the effectiveness of Multimodal Deep Learning in smart shopping and recommendation systems.

By combining visual and textual information, the system achieves more accurate and intelligent product matching compared to single-modality systems.
