# Emotion Detection Using Deep Learning (EfficientNet B0)

## 📖 Overview
This project focuses on building an **Emotion Detection** model using **deep learning** techniques.  
We use a **pre-trained EfficientNet B0** model to classify facial expressions into **7 categories** such as **happy, sad, angry, surprised, fearful, disgusted, and neutral**.

The model is fine-tuned on our custom emotion dataset.  
The project covers the **complete pipeline** from model building, training, evaluation, and making predictions on new images.

---

## 🛠️ Technologies Used
- Python 🐍
- PyTorch
- TIMM (PyTorch Image Models library)
- tqdm (for progress bars)
- NumPy
- Matplotlib (optional for visualization)

---

## 🚀 How It Works
1. **Model Building**
   - An EfficientNet B0 model is loaded with pre-trained ImageNet weights.
   - The classifier head is modified for **7 emotion classes**.

2. **Training**
   - The model is trained on the dataset using **Cross Entropy Loss** and **Adam Optimizer**.
   - Training and validation accuracies and losses are tracked for every epoch.
   - Best model weights (lowest validation loss) are saved automatically.

3. **Evaluation**
   - Model performance is evaluated using **accuracy score**, **confusion matrix**, and **classification report**.

4. **Inference**
   - Predict emotions for **new images** using the trained model.

---
