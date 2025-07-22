# RNN
# 🧠 Next Word Prediction Using RNN (Recurrent Neural Network)

This project builds a Recurrent Neural Network (RNN) using TensorFlow/Keras to predict the next word in a sentence. It leverages tokenization, text preprocessing, and sequence modeling to learn language patterns.

---

## 🚀 Features

- Uses `Tokenizer` for text preprocessing and word indexing
- Supports dynamic sequence generation from raw text
- Embeds input using Keras `Embedding` layer
- Predicts next word using `SimpleRNN` and `Dense` layers
- Offers `top-k` word predictions
- Includes methods to save and load trained models

---

## 🛠️ Tech Stack

- **Language**: Python
- **Libraries**: TensorFlow, NumPy
- **Model**: Sequential model with Embedding → SimpleRNN → Dense
- **Tokenizer**: Keras Tokenizer (with OOV handling)

---

## 📂 Files Included

- `next_word_predictor.py`: Complete class-based implementation
- `sample_texts`: Sample data to train on topics like AI, ML, NLP
- `model.h5`: Trained model (optional for saving/loading)
- `README.md`: Project documentation

---

## 📚 Workflow

1. **Preprocessing**
   - Remove punctuation, lowercase the text
   - Tokenize and create input-output word sequences

2. **Model Training**
   - Uses padded input sequences
   - One-hot encodes the next word as target
   - Trains RNN model using categorical cross-entropy

3. **Prediction**
   - Takes input phrase
   - Returns top N likely next words

---

## ✨ Example

```python
Input: "machine learning is"
Predicted next words: ['a', 'the', 'an']
