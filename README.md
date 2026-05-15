# 🍎 CNN-Based Fruit Classification

A deep learning-based image classification project developed for recognizing **10 different fruit categories** using a **Convolutional Neural Network (CNN)** architecture.  
The model performance was evaluated using **10-Fold Cross Validation**, achieving over **80% accuracy** on several data subsets.

---

# 📌 Project Overview

This project focuses on building an efficient and generalized fruit classification model using modern deep learning techniques.  
The dataset consists of images belonging to **10 distinct fruit classes**.

To ensure robust evaluation and minimize bias, the model was tested using the **10-Fold Cross Validation** technique. Experimental results demonstrated that the proposed architecture successfully exceeded the **80% accuracy threshold** on multiple validation folds.

---

# 🧠 Model Architecture & Techniques

The CNN architecture was carefully designed to improve classification performance while efficiently utilizing hardware resources.

## 🔹 Convolutional Neural Networks (CNN)

A multi-layer CNN architecture was implemented to hierarchically extract visual features such as:

- Texture
- Shape
- Color patterns

from fruit images.

---

## 🔹 Global Average Pooling (GAP)

Instead of using a traditional `Flatten` layer, **Global Average Pooling (GAP)** was applied.

### Advantages

- Reduces the number of trainable parameters
- Prevents overfitting
- Improves computational efficiency
- Reduces memory-related crashes

---

## 🔹 Batch Normalization

Batch Normalization layers were integrated into convolutional blocks to:

- Stabilize the training process
- Normalize feature distributions
- Accelerate convergence
- Improve overall learning efficiency

---

## 🔹 Dropout (0.6)

A high-rate dropout strategy (`0.6`) was used to prevent the model from memorizing training data.

### Benefits

- Enhances generalization capability
- Reduces overfitting
- Improves validation accuracy performance

---

# 📊 Data Preprocessing & Training Strategies

## 🔹 Data Augmentation

To improve model robustness against different image conditions, several augmentation techniques were applied:

- Rotation
- Horizontal shifting
- Flipping / Mirroring

These transformations increased dataset diversity and improved generalization.

---

## 🔹 Early Stopping

The training process was monitored using **Early Stopping** with `restore_best_weights=True`.

This allowed the model to:

- Preserve the best-performing weights
- Stop training when performance stagnated
- Prevent unnecessary computation and overfitting

---

## 🔹 ReduceLROnPlateau

A dynamic learning rate reduction strategy was used during training.

When the loss function stopped improving:

- The learning rate was automatically decreased
- The optimizer was able to escape local minima
- More stable convergence was achieved

---

# 📈 Performance Analysis

During the 10-Fold Cross Validation process:

- The model successfully exceeded **80% accuracy** on several validation subsets.
- The highest recorded accuracy demonstrated the effectiveness of the proposed CNN architecture.
- Consistent fold performances indicated that techniques such as:
  - Global Average Pooling
  - Dropout
  - Batch Normalization

positively contributed to the model’s generalization capability.

---

# 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn

---

# 🚀 Features

- ✅ Deep Learning-based Fruit Classification
- ✅ 10 Different Fruit Categories
- ✅ CNN Architecture Optimization
- ✅ 10-Fold Cross Validation
- ✅ Data Augmentation Support
- ✅ Overfitting Prevention Techniques
- ✅ Dynamic Learning Rate Scheduling

---

# 📂 Project Structure

```bash
├── dataset/
├── models/
├── notebooks/
├── results/
├── train.py
├── evaluate.py
├── requirements.txt
└── README.md
```

---

# 📌 Future Improvements

- Transfer Learning Integration (ResNet, EfficientNet, MobileNet)
- Larger and more diverse fruit datasets
- Real-time fruit detection support
- Mobile deployment optimization

---

# 📜 Conclusion

This project demonstrates the effectiveness of CNN-based architectures for fruit image classification tasks.  
The combination of advanced regularization methods, preprocessing strategies, and cross-validation techniques resulted in a stable and successful deep learning model with strong generalization performance.
