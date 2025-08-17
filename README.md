# 📝 Next Word Predictor (LSTM-based)

A deep learning project that predicts the next word in a sequence using an **LSTM (Long Short-Term Memory)** model.  
This project demonstrates how recurrent neural networks can learn language context and improve predictive text generation.

---

## 🚀 Overview

The **Next Word Predictor** leverages an **LSTM-based neural network** to model sequential dependencies in text data.  
It takes a sequence of words as input and predicts the **most likely next word**, making it suitable for applications such as:

- Predictive typing (like in keyboards)  
- Smart text editors  
- Chatbots & conversational AI  
- Writing assistance tools  

---

## ✨ Features

- LSTM-based sequence modeling for language prediction.  
- Preprocessing with tokenization and sequence padding.  
- Trainable on any custom text dataset.  
- Real-time next word prediction with trained weights.  
- Simple and modular code structure for easy experimentation.  

---

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/AshutoshSingh840/Next_Word_Predictor.git
cd Next_Word_Predictor
```
2. Install dependencies:

```bash
pip install -r requirements.txt
```
# 🛠️ Usage
Training the Model
Prepare your dataset (plain text file, one sentence per line).
Run:
```bash
python train.py --data data/corpus.txt --save-path model.h5
```

Predicting Next Word
```python```
from model import NextWordPredictor

Load the trained LSTM model
predictor = NextWordPredictor(model_path="model.h5", tokenizer_path="tokenizer.pkl")

Predict the next word
input_text = "The quick brown"
print("Prediction:", predictor.predict_next(input_text))

# 📊 Model Details

Architecture:

  • Embedding layer
  • LSTM layers (1–2 stacked)
  • Dense + Softmax output layer
  • Loss Function: Categorical Crossentropy
  • Optimizer: Adam
  • Metrics: Accuracy

# 📈 Results
 • Training and evaluation results of the LSTM-based Next Word Predictor:
 • Model improves steadily over 50 epochs.
 • Loss decreases while accuracy increases, showing the model’s ability to learn sequential dependencies.

# 🤝 Contribution
Contributions are welcome!
Follow these steps:

• Fork the repo
• Create a branch (git checkout -b feature-name)
• Commit changes (git commit -m "Add feature")
• Push branch (git push origin feature-name)
• Create a Pull Request

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

