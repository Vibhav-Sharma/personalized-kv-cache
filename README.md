# 🧠 Personalization-Aware KV Cache Eviction in LLMs

This is a research-driven project that explores **memory optimization in Large Language Models (LLMs)** using **user personalization**. The goal is to retain user-relevant tokens in cache based on their interaction history, improving both efficiency and relevance of the responses.

---

## 🔍 Project Overview

Most current cache eviction techniques in LLMs (like FIFO or attention-based) do not consider **who the user is**. This project introduces a lightweight **topic classifier** that tags user queries and helps the model prioritize what topics to keep in memory, inspired by behavior-driven personalization.

---

## 🧪 Features

- ✅ Manual prompt dataset creation (LLMs, Valorant, Weight Loss).
- ✅ Training a logistic regression model using TF-IDF features.
- ✅ Achieved **94% accuracy** in classifying user prompts.
- ✅ Visualized predictions with confusion matrix and graphs.
- 🧠 *Next steps*: Use the classifier output to guide KV cache eviction.

---

## 📊 Sample Prompt Dataset

| Prompt                                  | Topic        |
|----------------------------------------|--------------|
| How to fine-tune LLaMA 3?              | llm          |
| Best crosshair for Valorant beginners? | valorant     |
| Foods to avoid for weight loss         | weight_loss  |

---

## 🛠️ Tech Stack

- Python (3.11+)
- Google Colab
- pandas, scikit-learn, matplotlib, numpy

---

## 📁 Project Files

- `personalized_kv_cache_eviction.ipynb` — Main notebook  
- `requirements.txt` — Dependencies  
- *(optional)* `data/` — Prompt dataset  
- *(optional)* `images/` — Confusion matrix and plots

---

## 📚 Future Work

- Phase 2: Behavioral tracking of users' topic frequencies
- Phase 3: Personalized token retention engine for LLM cache
- Phase 4: Integration with transformer inference pipelines

---

## 📜 License

MIT License – feel free to use, cite, or extend this project with credit.

---

### 👤 Author

**Vibhav Sharma**  
B.Tech CSE, VIT Chennai  
Passionate about LLMs, optimization, and human-AI interaction

---

> “Memory isn’t about what’s old. It’s about what matters.”
