# Kenyan Generative Literature with TensorFlow

This project explores how **Generative AI** can be used to create **engaging, Kenyan-themed literature** using a **character-level LSTM model** built with TensorFlow and Keras.



## 🎯 Objective

To generate culturally rooted, thought-provoking literary text by training a neural network on a small, curated Kenyan corpus — fulfilling the task:

> **"Generate a new type of literature that is both engaging and thought-provoking."**

---

## 🧠 Model Summary

- **Tokenization**: Character-level (ideal for small text datasets)
- **Model Type**: LSTM (Long Short-Term Memory)
- **Loss**: Categorical Crossentropy
- **Optimizer**: Adam
- **Training Method**: EarlyStopping to prevent overfitting

### Architecture

```text
Input: 40-character sliding window (one-hot encoded)
Model:
  → LSTM(128 units)
  → Dropout(0.2)
  → Dense(vocab
_size, activation='softmax')
