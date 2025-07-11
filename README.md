# 🍽️ Ghanaian Food Image Classifier

This project implements a deep learning model that classifies images of **Ghanaian food** using computer vision. The model is trained in the `food_vision.ipynb` notebook and leverages transfer learning with a powerful pretrained CNN backbone.

---

## 📚 Project Overview

- 🇬🇭 Focus: Classifying popular Ghanaian dishes from images
- 🧠 Model: CNN with transfer learning (e.g., ResNet or EfficientNet)
- 📁 Framework: Built using PyTorch
- 🏷️ Classes: Multiple Ghanaian food categories (e.g., jollof, waakye, kenkey, banku, fufu, etc.)
- 🎯 Goal: Build an image classifier to support food recognition apps, health tracking tools, or cultural promotion platforms

---

## 🗂️ Dataset

The dataset consists of images of various Ghanaian food items. Images were collected from diverse sources to capture:
- Different lighting conditions
- Realistic settings (restaurants, home kitchens, outdoor)
- Various angles and food arrangements

Each image is labeled with its corresponding dish name.

> **Note:** Dataset is organized into folders by class, e.g.:
```
data/
  train/
    jollof/
    kenkey/
    banku/
    ...
  val/
  test/
```

---

## 🧠 Model Architecture

- Input size: Resized images (e.g., 224x224)
- Model: Pretrained ResNet-50 (or other backbone)
- Output: Softmax layer with N units (N = number of food classes)
- Loss: CrossEntropyLoss
- Optimizer: Adam or SGD

---

## 🛠️ How to Run

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/ghanaian-food-classifier.git
cd ghanaian-food-classifier
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the notebook
```bash
jupyter notebook food_vision.ipynb
```

---

## 🚀 Features

- ✅ Accurate Ghanaian food classification
- ✅ Uses transfer learning for improved accuracy with limited data
- ✅ Data augmentation to improve generalization
- ✅ Training, validation, and test evaluation
- ✅ Option to export trained model

---

## 📊 Evaluation

- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- Visualizations of predictions

---

## 📦 Potential Applications

- 🍱 Nutrition tracking apps
- 📱 Mobile food recognition tools
- 🌍 Promoting Ghanaian culture and cuisine
- 📊 Restaurant menu auto-tagging
- 🔬 Food AI research in underrepresented cuisines

---

## 🤝 Acknowledgments

- Dataset curated from publicly available images and original sources
- Inspired by [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) and adapted for Ghanaian cuisine

---

## 📌 Future Work

- Deploy the model using Streamlit or Flask
- Extend to multilabel classification (e.g., combo meals)
- Add calorie/nutrition estimates based on predicted class