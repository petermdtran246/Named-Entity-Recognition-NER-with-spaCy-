# 🧠 Named Entity Recognition (NER) with spaCy  
A simple but powerful demonstration of **Named Entity Recognition (NER)** using **spaCy**.  
This project showcases how different preprocessing steps (raw vs cleaned text) affect the accuracy of entity extraction.

---

## 🚀 Overview  
NER is the task of identifying *important, real-world entities* in text such as:

- 👤 People  
- 🌍 Locations  
- 🏢 Organizations  
- 📅 Dates  
- 💰 Monetary values  

This project uses spaCy’s pre-trained **`en_core_web_sm`** model to extract entities from a sample Wikipedia-style paragraph about **Apple Inc.**

It also compares:

### 🔹 **NER on raw text**  
vs  
### 🔹 **NER on cleaned text (lowercased + punctuation removed)**  

This demonstrates a key NLP lesson:

> **“Cleaning text too aggressively can remove information that NER models rely on.”**

---

## 📂 Project Structure  
📁 ner_spacy_project
│── ner_apple.ipynb # Full Jupyter script with comments
│── README.md # Documentation (this file)



📊 Example Output (Raw Text)
Apple Inc. → ORG
April 1, 1976 → DATE
Steve Jobs → PERSON
Steve Wozniak → PERSON
Ronald Wayne → PERSON
Los Altos → GPE
California → GPE
...

NER performs strongly because the text maintains structure and capitalization.

📉 Example Output (Cleaned Text)
apple inc → ORG
april 1 1976 → DATE
steve jobs → PERSON
...

You will notice:

• Some entities disappear

• Some entities merge incorrectly

• Some labels are less accurate

This demonstrates that NER models rely on punctuation and capitalization.

