# 🧠 Brain Tumor Classification using Ensemble Learning

This project classifies brain MRI images into four categories using an **ensemble of deep learning models**: **ANN**, **CNN**, and **EfficientNetB0**. By leveraging the unique strengths of each model, the ensemble approach achieves high accuracy and robustness in predictions.

---

## 📌 Tumor Categories
The classification system distinguishes between the following tumor types:
- 🧠 **Glioma Tumor** – Tumors originating in the glial cells of the brain.
- 🧠 **Meningioma Tumor** – Tumors developing in the meninges (membranes surrounding the brain and spinal cord).
- 🧠 **Pituitary Tumor** – Abnormal growths in the pituitary gland.
- ✅ **No Tumor** – Healthy brain MRIs without any tumors.

---

## ⚙️ Models Used

### 🔹 1. ANN (Artificial Neural Network)
- Simple dense layers with ReLU activations.
- Input: Flattened MRI image vectors.
- Lightweight and faster.

### 🔹 2. CNN (Convolutional Neural Network)
- Custom convolutional layers for spatial feature extraction.
- Learns tumor patterns directly from image data.

### 🔹 3. EfficientNetB0 (Transfer Learning)
- Pretrained on ImageNet, fine-tuned on MRI dataset.
- Efficient performance with fewer parameters.

### 🔹 4. Ensemble Model (Majority Voting)
- Combines predictions from ANN, CNN, and EfficientNetB0.
- Uses majority voting to decide the final class.
- More robust to overfitting and model-specific errors.

## 🗂 Dataset Structure
```
Testing/
├── glioma tumor/
├── meningioma tumor/
├── no tumor/
└── pituitary tumor/
```

## 🚀 How to Run

1. **Clone the repo**  
   `git clone https://github.com/yourusername/brain-tumor-classification.git`

2. **Install dependencies**  
   `pip install -r requirements.txt`

3. **Predict tumor type**  
   `python predict.py --image_path "Testing/no tumor/example.jpg"`

4. **(Optional) Run Web App**  
   `cd webapp && python app.py`  
   Open `http://localhost:5000` in browser.

## 📊 Accuracy
- ANN: ~90%  
- CNN: ~94%  
- EfficientNetB0: ~96%  
- **Ensemble: ~97%**

## 👨‍💻 Author
**Gundreddy Muralidhar Reddy**  

> ⚠️ *For academic use only. Not intended for real-world medical diagnosis.*
