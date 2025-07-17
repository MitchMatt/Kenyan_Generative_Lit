# 🇰🇪 Kenyan Generative Literature with TensorFlow

This project explores how **Generative AI** can be used to create **engaging, Kenyan-themed literature** using a **character-level LSTM model** built with TensorFlow and Keras.

---

## 🎯 Objective

To generate culturally rooted, thought-provoking literary text by training a neural network on a small, curated Kenyan corpus, fulfilling the task:

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
  → Dense(vocab_size, activation='softmax')
````

---

## 📚 Dataset

A handcrafted Kenyan-themed corpus with references to:

* Nairobi streets and matatus
* Kisumu markets and Luo songs
* Mombasa dhows and Swahili kitchens
* Rift Valley landscapes
* Maasai warriors and Kericho tea
* Kibera, Eldoret, Kitui, and more

Example snippet from corpus:

> “On Lake Victoria, fishermen sang haunting Luo songs.”
> “Nairobi streets buzzed with matatus and the chatter of street vendors.”
> “Under baobab trees, elders passed down stories like treasures.”

---

## 🚀 Usage

### 1. Clone this repo and open the notebook:

```bash
git clone https://github.com/yourusername/kenyan-generative-literature
cd kenyan-generative-literature
```

### 2. Run the Jupyter Notebook:

```bash
Jupyter Notebook Kenyan_Generative_Literature_TF.ipynb
```

### 3. Generate Literature:

Use the helper function to generate text:

```python
generate_text("elders gathered under baobab trees")
```

---

## 🖊️ Sample Output

Given the seed:
`"Nairobi streets buzzed with matatus"`

Example generated text:

> *"Nairobi streets buzzed with matatus and the chatter of street vendors under the sun and into the rift."*

(Note: Output may vary with temperature settings and training.)

---

## 📦 Dependencies

* Python 3.8+
* TensorFlow 2.x
* NumPy

Install with:

```bash
pip install tensorflow numpy
```

---

## ✅ Assignment Alignment

* ✔️ Task: Generative Literature (Engaging + Thought-provoking)
* ✔️ Tool: TensorFlow + Keras
* ✔️ Output: Kenyan-style text generation
* ✔️ Included: Code, Output, Notebook

---

## 📄 License

This project is part of a class assignment under the EBU CDA302/MSDA302 Deep Learning with TensorFlow module. For academic and educational use.

---

## 🙌 Acknowledgements

Special thanks to:

* The Kenyan landscapes, cultures, and voices that inspired this corpus
* TensorFlow/Keras open-source community
