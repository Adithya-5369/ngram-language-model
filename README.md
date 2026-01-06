# 5-gram Language Model for Literary Style Text Generation

This project implements a **5-gram (n=5) Language Model** and trains it on classic literature from **Project Gutenberg** to generate text in the style of a chosen author.  
Given a short input prompt, the model continues the text using learned n-gram probabilities.

In this implementation, the model is trained on **Jane Austen's "Emma"**.

---

## 📌 Problem Statement

Implement an n-gram Language Model with **n = 5** and generate text in the style of a chosen author using books from Project Gutenberg.

Example:
```

Input: "The day was very ..."
Output: (generated continuation in the author's style)

````

The model is tested on **at least three different input prompts**.

---

## 📚 Dataset

- Source: **Project Gutenberg** (via NLTK Gutenberg corpus)
- Author used: **Jane Austen**
- Book: *Emma*

The dataset is automatically downloaded using NLTK.

---

## 🧠 Methodology

### 5-gram Language Model

- The model uses a **sliding window of 5 words**
- The first **4 words are the context**
- The **5th word is predicted** based on frequency counts
- During generation:
  - The next word is sampled **probabilistically** from the learned distribution
  - The generated word is appended and the window slides forward

---

## 🛠️ Tech Stack

- Python
- NLTK
- Jupyter Notebook

---

## 🚀 How to Run

### 1. Install dependencies

```bash
pip install nltk jupyter
````

### 2. Run the notebook

```bash
jupyter notebook
```

Open:

```
ngram_lm.ipynb
```

The notebook will automatically download the required Gutenberg dataset.

---

## 🧪 Sample Prompts Used

```
"The day was very"
"Deep into that"
"It was a"
```

The model generates continuations in the style of Jane Austen.

---

## 📁 Project Structure

```
ngram-language-model/
│
├── ngram_lm.ipynb
└── README.md
```

---

## 🧠 Key Learnings

* How n-gram language models work
* How text generation can be done using probability distributions
* Limitations of n-gram models (repetition, local coherence only)
* How writing style can be mimicked using statistical language models

---

## ⚠️ Limitations

* No long-term coherence (n-gram limitation)
* Sensitive to training data size
* May repeat phrases or stop abruptly

---

## 📖 References

* Jurafsky & Martin, *Speech and Language Processing*
* Project Gutenberg: [https://www.gutenberg.org/](https://www.gutenberg.org/)
* NLTK Documentation: [https://www.nltk.org/](https://www.nltk.org/)

---

## 🛡 License

This project is licensed under the [MIT License](LICENSE).  
You are free to use, modify, and distribute this code with attribution.

---

## Author

**Adithya Sai Srinivas**  
📧 muttaadithyasaisrinivas@gmail.com  
🌐 [Portfolio](https://adithya369.pages.dev) • [LinkedIn](https://linkedin.com/in/adithyasaisrinivas)
