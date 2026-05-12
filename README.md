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



## 🔹 Experimental & Comparative Analysis


| Model               | Type                 | Main Role                        | Accuracy / Metric | Loss   | Notes                                                          |
| ------------------- | -------------------- | -------------------------------- | ----------------- | ------ | -------------------------------------------------------------- |
| ResNet50            | CNN                  | Image Feature Extraction         | 99.15%            | 0.0406 | Achieved the highest image classification performance          |
| EfficientNet        | CNN                  | Lightweight Image Classification | 71.90%            | 0.8403 | Faster and more efficient with lower accuracy                  |
| GRU                 | RNN                  | Text Feature Extraction          | 85.95%            | 0.2186 | Good performance for text sequence understanding               |
| LSTM                | RNN                  | Advanced Text Encoding           | 89.39%            | 0.37  | Better handling of long-term dependencies                      |
| Concatenation Model | Fusion Model         | Combine image and text features  | —                 | —      | Merged visual and textual embeddings into one feature vector   |
| Similarity Model    | Recommendation Model | Product matching and ranking     | Cosine Similarity | —      | Ranked products according to similarity between image and text |



---



## 🔹 Teamwork & Individual Contribution

| Team Member | Contribution |
|---|---|
| Ibrahim | Built and trained the ResNet50 image classification model |
| Ahmed | Developed the EfficientNet model and optimized image preprocessing |
| Yasmin | Implemented the GRU text feature extraction model |
| Omnya | Developed and trained the LSTM text encoder |
| Mohamed | Built the Concatenation Fusion Model for combining image and text embeddings |
| Shouk | Implemented the Similarity Model using Cosine Similarity and product ranking |



---



## 🔹 Evaluation Metrics & Validation Strategy

- The models were evaluated using Accuracy and Loss metrics.
- Validation datasets were used during training to monitor model generalization.
- Early Stopping was applied to reduce overfitting and restore the best model weights.
- Training and validation accuracy/loss curves were analyzed for performance monitoring.
- Cosine Similarity was used to measure similarity between image and text embeddings in the recommendation stage.
- Data preprocessing techniques such as image resizing, normalization, tokenization, and sequence padding were applied before training.



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
