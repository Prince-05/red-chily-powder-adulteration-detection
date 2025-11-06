# 🌶️ Red Chilli Adulteration Detection

This project aims to detect adulteration in **red chilli powder** using **deep learning models**.  
It leverages image-based analysis to distinguish **pure chilli powder** from **adulterated samples** (e.g., mixed with brick powder).

---

## 📘 Project Overview

Adulteration of food products is a major public health issue.  
This project applies **computer vision** and **explainable AI (XAI)** techniques to identify adulterated red chilli powder from images.

The notebook demonstrates:
- Data loading and preprocessing of chilli powder images.
- Building and fine-tuning pretrained CNN models.
- Model interpretability using **Captum**.
- Evaluation and visualization of predictions.

---

## 🧠 Key Features

- **PyTorch + timm** for deep learning.
- **Captum** for model explainability (feature attribution).
- **Train/Test split** for fair model evaluation.
- **Custom PyTorch Dataset** for efficient data loading.
- GPU support for faster training.

---

## 🗂️ Dataset

The dataset used is:
```
Dataset for Adulterated Red Chilli Powder with Brick Powder
```

It contains two categories:
- `Pure` – images of pure red chilli powder  
- `Adulterated` – images of red chilli powder mixed with brick powder

> Ensure that your dataset directory structure matches what the notebook expects.

---

## ⚙️ Project Workflow

1. **Import Libraries**  
   Loads essential packages like `torch`, `numpy`, `matplotlib`, `captum`, and `timm`.

2. **Setup Device & Seed**  
   Ensures reproducibility and utilizes GPU (if available).

3. **Data Loading**  
   - Scans dataset directory.
   - Maps file paths and labels.
   - Defines a custom `ChilliDataset` class.

4. **Data Splitting**  
   Uses `train_test_split` for stratified splitting.

5. **Model Definition**  
   Builds model using pretrained architecture (e.g., `ResNet`, `EfficientNet`) via **timm**.

6. **Training & Evaluation**  
   - Trains the CNN on training data.
   - Evaluates using accuracy and loss metrics.

7. **Explainable AI (Captum)**  
   Visualizes which image regions contribute most to model predictions.

---

## 🧩 Dependencies

Install the required libraries before running the notebook:

```bash
pip install torch torchvision timm captum matplotlib numpy scikit-learn
```

---

## 🚀 How to Run

1. Clone or download this repository.
2. Place the dataset folder in the project root.
3. Open the notebook in **Jupyter** or **Google Colab**.
4. Run all cells sequentially.

---

## 🧾 Results

- Models trained on chilli powder images achieve high classification accuracy.
- Captum visualizations highlight the color and texture regions influencing predictions.

---

## 🧑‍🔬 Future Work

- Extend to other food adulteration types (turmeric, milk, etc.)
- Integrate with a mobile or web app for real-time adulteration detection.

---

## 🖋️ Author

**Prince Saini**  
Machine Learning & Computer Vision Researcher  

---

## 🪪 License

This project is open-sourced under the **MIT License**.

---
