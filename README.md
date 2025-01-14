# **Shakespeare Text Prediction Using LSTM**

This project demonstrates text generation in Shakespearean style using a **Long Short-Term Memory (LSTM)** neural network. The model learns to predict and generate text based on patterns and language structures in Shakespeare's works.

---

## **How It Works**

### **1. Data Preprocessing**
The first step involves preparing the Shakespearean text dataset for training:
- The text is cleaned and converted to lowercase for consistency.
- It is then tokenized into sequences of characters or words.
- Each sequence is mapped into input-output pairs:
  - **Input**: A sequence of characters/words.
  - **Output**: The next character/word following the sequence.

---

### **2. Model Architecture**
The core of the project is an **LSTM-based neural network**:
- **Embedding Layer**: Converts input tokens into dense numerical vectors.
- **LSTM Layers**: Processes sequential data, learning dependencies and language structure.
- **Dense Output Layer**: Predicts the probability distribution of the next character or word.

The LSTM’s ability to retain context over long sequences allows it to capture Shakespearean writing style effectively.

---

### **3. Training Process**
The model is trained on sequences of Shakespeare’s text to predict the next character or word:
- The **loss function** minimizes the error between the predicted and actual next character/word.
- Training continues until the model learns to replicate the structure and tone of Shakespeare’s works.

---

### **4. Text Generation**
Once trained, the model generates text in the following way:
1. **Input Prompt**: The user provides a starting sequence (e.g., `"To be or not to be"`).
2. **Prediction Loop**:
   - The model predicts the next character/word based on the input.
   - The prediction is appended to the input sequence.
   - This updated sequence is used to predict the next character/word.
3. **Output**:
   - The process continues iteratively until the desired length of text is generated.

---

### **Key Output**
- **Generated Shakespearean Text**:
   - Starting with a prompt, the model produces a sequence that mimics Shakespeare’s writing style.
