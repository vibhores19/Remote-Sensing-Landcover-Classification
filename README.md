# Remote-Sensing-Landcover-Classification
A machine learning and deep learning-based framework for classifying remote sensing data from Landsat 5 in mountainous Colorado. Includes traditional ML models (SVM, RF, DT) and deep learning architectures (CNN, LSTM, ResNet) to classify 14 land cover types with high accuracy.


# 🛰️ Classifying Remote Sensing Data using ML and DL Techniques

This repository presents a classification framework for identifying land cover types in rugged, mountainous terrain using satellite imagery from Landsat 5. The project leverages traditional machine learning and deep learning algorithms, including **Random Forest**, **SVM**, **Decision Trees**, **CNN**, **LSTM**, and **ResNet**, to classify 14 ground cover classes from spectral band data.

---

## 📌 Project Summary

- **Dataset**: Landsat 5 satellite imagery from a mountainous region in Colorado
- **Samples**: 15,000 labeled instances + 3.4 million unlabeled instances
- **Bands**: Six spectral bands used (bands 1–5 and 7)
- **Target**: 14 distinct ground cover classes

This project aims to improve accuracy and automation in remote sensing data classification—especially for complex, uneven terrain—using scalable and high-performance models.

---

## 🧠 Models Used

| Model        | Type          | Strengths                          |
|--------------|---------------|------------------------------------|
| Decision Tree| Traditional ML| Fast and interpretable             |
| Random Forest| Traditional ML| Handles imbalance, reduces overfit |
| SVM          | Traditional ML| Best performance among ML models   |
| CNN          | Deep Learning | Best performing DL model (97%)     |
| LSTM         | Deep Learning | Captures sequential relationships  |
| ResNet       | Deep Learning | Deeper learning, skip connections  |

---

## 🧪 Methodology

1. **Preprocessing**: Cleaned and labeled columns for spectral bands, normalized data.
2. **Model Training**:
   - Tuned ML models using Grid Search CV.
   - Applied hyperparameter optimization on DL models (layer depth, batch size, dropout).
3. **Evaluation Metrics**:
   - Accuracy, Precision, Recall, F1 Score
4. **Prediction on Unlabeled Data**:
   - CNN was used to classify the 3.4 million unlabeled instances.

---

## 📈 Key Results

| Model   | Final Accuracy | Final F1 Score |
|---------|----------------|----------------|
| RF      | 93%            | 92%            |
| DT      | 89%            | 87%            |
| SVM     | 97%            | 96%            |
| CNN     | 97%            | 96%            |
| LSTM    | 96%            | 94%            |
| ResNet  | 89%            | 87%            |

- **Best Performer**: CNN selected as final model due to better generalizability and performance on unstructured image data.

---

## 🌍 Class Distribution

Example ground cover classes:

- Scotch Pine  
- Douglas Fir  
- Aspen  
- Water  
- Dry Meadow  
- Bushland  
- Alpine Vegetation  
*(Full list available in the report.)*

---

## 🖼️ Visualizations

- Training vs Validation Accuracy & Loss graphs
- Classification reports
- Predicted class distribution of 3.4M unlabeled samples

---

## 📚 Future Work

- Use of larger, more balanced training datasets
- Explore CNN hybrids and transformer-based models
- Implement transfer learning with pre-trained satellite models
- Introduce spectral-temporal fusion techniques
- Improve misclassification handling via synthetic data augmentation

---
