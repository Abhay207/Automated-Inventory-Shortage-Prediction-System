# Smart-Inventory-Shortage-Prediction-Suite

This project predicts supply shortages using a combination of LSTM, XGBoost, and hybrid models, tailored to handle highly imbalanced datasets. It also features a Retrieval-Augmented Generation (RAG) based chatbot that offers real-time, context-aware insights into shortage causes.

---

## 📚 Table of Contents

- [📌 Project Overview](#-project-overview)
- [🧠 Models Used](#-models-used)
- [⚙️ Tech Stack](#️-tech-stack)
- [📊 Performance](#-performance)
- [🚀 Getting Started](#-getting-started)
  - [🔧 Installation](#-installation)
  - [▶️ How to Run](#️-how-to-run)
  - [🌐 Web Interface](#-web-interface)
  - [🙌 Acknowledgements](#-acknowledgements)
- [📝 License](#-license)

---

## 📌 Project Overview

This project delivers a multi-model solution to supply chain shortage prediction using sequence-based deep learning and boosting methods. It is optimized for high performance on imbalanced datasets and supports dynamic reasoning through a chatbot interface.

---

## 🧠 Models Used

| Model Type              | Optimization Target | Use Case                        |
|-------------------------|---------------------|---------------------------------|
| LSTM + XGBoost Hybrid   | Balanced F1-score   | General predictions             |
| XGBoost (High Recall)   | High Recall         | Critical items                  |
| XGBoost (High Precision)| High Precision      | Low-impact items                |

---

## ⚙️ Tech Stack

- **Modeling**: TensorFlow, XGBoost
- **API**: FastAPI
- **Chatbot**: LangChain, ChromaDB, HuggingFace Embeddings
- **LLM**: llama-2-7b-chat.ggmlv3.q4_0 via HuggingFace 
- **Deployment**: FastAPI endpoints
- **Web Interface**: By collaborator
---

## 📊 Performance

- Precision: up to **0.95**
- Accuracy: up to **0.98**
- Custom thresholds selected for each model to improve classification on highly imbalanced data.

---

## 🚀 Getting Started

### 🔧 Installation

```bash
git clone https://github.com/Abhay207/Automated-Inventory-Shortage-Prediction-System.git
cd Automated-Inventory-Shortage-Prediction-System
pip install -r requirements.txt
```

### ▶️ How to Run

Start the FastAPI server locally:

```bash
uvicorn main:app --reload
```

### 🌐 Web Interface
A ready-to-use web interface is available in the following GitHub repository. [👉 View the GitHub Repository](https://github.com/AsharSi/stock-prediction)

. It was developed by a collaborator to provide a user-friendly dashboard for interacting with the models and chatbot.

### 🙌 Acknowledgements
- Web UI developed by AsharSi

- Powered by HuggingFace Transformers, LangChain, ChromaDB, and FastAPI

- Special thanks to the open-source ecosystem

## 📝 License
This project is licensed under the MIT License.
