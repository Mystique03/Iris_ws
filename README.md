---

# 🩺 Iris — Voice Assistant for Disease Diagnosis using ML & NLP

<p align="center">
An AI-powered voice assistant that predicts diseases from spoken symptoms using Machine Learning and NLP, and provides personalized treatment & dietary recommendations via LLM integration.
</p>

---

## 🔍 Project Overview

**Iris** is a healthcare-focused **Voice Assistant system** designed to assist in early disease detection, particularly for **remote and underserved regions** where medical access is limited.

Users speak their symptoms naturally, and the system:

1. Converts voice input to text using Speech Recognition
2. Predicts the most likely disease using a **Random Forest classifier trained on symptom–disease data**
3. Retrieves **treatment and diet recommendations using OpenAI's API**
4. Communicates results back through voice using **Text-to-Speech synthesis**

This project demonstrates the integration of:

* Machine Learning disease classification
* Natural Language Processing pipelines
* Speech-to-Text & Text-to-Speech engines
* LLM-powered medical information retrieval

---

## 🚀 Key Features

* 🎙 **Voice-based interaction** (Speech → Text → Prediction → Spoken response)
* 🧠 **ML-based disease prediction** using Random Forest
* 📊 **132 symptoms mapped to 41 diseases**
* 🗣 **NLP pipeline** for speech understanding
* 🔊 **Human-like voice responses** via Pyttsx3
* 🤖 **LLM-powered recommendations** for:

  * Treatment suggestions
  * Diet plans
* 🌍 Designed for **remote healthcare assistance**

---

## 🏗 System Architecture

```
User Voice Input
        │
        ▼
Speech Recognition (Speech → Text)
        │
        ▼
NLP Processing & Feature Mapping
        │
        ▼
Random Forest Classifier
        │
        ▼
Disease Prediction
        │
 ┌──────┴────────┐
 │               │
 ▼               ▼
OpenAI LLM       Pyttsx3
(Treatments &   (Text → Speech)
Diet Retrieval)
        │
        ▼
Voice Output to User
```

---

## 🗂 Dataset Overview

* **Source:** Kaggle healthcare datasets
* **Features:**

  * 132 symptom inputs
  * Cleaned & normalized via preprocessing
* **Targets:**

  * 41 unique diseases
* **Privacy:**

  * No personal identifiers (no names, IDs, or phone numbers)

---

## 🤖 Machine Learning Model

We evaluated several supervised ML algorithms:

* Support Vector Machine (SVM)
* Naïve Bayes
* Decision Tree
* ✅ **Random Forest (best performer)**

### Final Model:

* **Random Forest Classifier**
* Chosen for:

  * Higher accuracy
  * Robust handling of noisy symptom data
  * Interpretability

**Model Performance:**

* ✅ **92.68% accuracy** on held-out test data

---

## ⚙️ Tech Stack

### Programming

* Python

### Machine Learning & NLP

* Scikit-learn
* Random Forest
* NLTK

### Speech Processing

* `SpeechRecognition` (Speech → Text)
* `pyttsx3` (Text → Speech)

### LLM Integration

* **OpenAI API**

  * Used for treatment & dietary recommendation retrieval

---

## 🛠 Workflow

```plaintext
1. Collect symptom dataset
2. Clean & preprocess data
3. Train/test ML models
4. Select best-performing algorithm (Random Forest)
5. Integrate voice input with SpeechRecognition
6. Generate spoken responses with pyttsx3
7. Query OpenAI for diet & treatment information
8. Deploy interactive assistant pipeline
```

---

## 💻 Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/iris-voice-assistant.git
cd iris-voice-assistant
```

### 2️⃣ Install Requirements

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure OpenAI API

Create a `.env` file:

```env
OPENAI_API_KEY=your_api_key_here
```

---

## ▶️ Running the Application

```bash
python main.py
```

🎧 Speak your symptoms when prompted and receive diagnosis and recommendations verbally.

---

## 📈 Results

| Component             | Performance                                 |
| --------------------- | ------------------------------------------- |
| Disease Prediction    | **92.68% accuracy**                         |
| Speech Recognition    | High transcription accuracy                 |
| Text-to-Speech Output | Clear verbal responses                      |
| LLM Recommendations   | Relevant & actionable treatment suggestions |

---

## 📄 Related Publication

This project is based on the peer-reviewed conference paper:

> **Voice Assistant for Disease Diagnosis Using Machine Learning and Natural Language Processing**
> Smitha Reddy S. et al., NCRACIT
> *(Methodology & evaluation details derived from this work.)*

---

## 🌟 Applications

* Rural telemedicine support
* Healthcare kiosks & mobile health tools
* Medical triage aids
* Elderly care voice assistants
* Educational healthcare demos

---

## 🔮 Future Enhancements

* ✅ Expand dataset to cover more diseases
* 🌐 Multilingual voice input
* 📷 Integration of medical image diagnosis
* 🧠 Deep learning-based symptom understanding
* 🏥 Clinical decision support system integration


---


