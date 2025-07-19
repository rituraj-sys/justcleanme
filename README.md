# justcleanme 🧹

A lightweight Python package for quick and beginner-friendly NLP text preprocessing. Includes common text cleaning utilities like removing punctuation, emojis, stopwords, correcting spelling, converting to TF-IDF, and more — all wrapped in a simple class `TextCleaner`.

---

## 🚀 Installation

Install via pip:

```bash
pip install justcleanme
```

Or if you're installing from a local build:

```bash
pip install dist/justcleanme-0.1.0.tar.gz
```

---

## 🧰 Features

- Word Count
- Punctuation Removal
- Emoji Removal
- Stopword Removal
- Spelling Correction
- HTML Entity Cleaning
- TF-IDF Vectorization

---

## 🧪 Usage Example

```python
from justcleanme import TextCleaner

cleaner = TextCleaner()
text = "Hello 👋!!! This is <b>sample</b> text with stopwords, emojis 😅 and HTML entities &amp; punctuation!"

# Count words
print(cleaner.count_words(text))  # ➜ Number of words

# Remove punctuation
print(cleaner.remove_punctuation(text))

# Remove emojis
print(cleaner.remove_emojis(text))

# Remove stopwords
print(cleaner.remove_stopwords(text))

# Correct spelling
print(cleaner.correct_spelling("Ths is a smple txt"))

# Remove HTML entities
print(cleaner.remove_html("Stay &amp; safe"))

# TF-IDF Vectorization
texts = ["This is sentence one", "And here is sentence two"]
tfidf_matrix = cleaner.convert_to_tfidf(texts)
print(tfidf_matrix.toarray())
```

---

## 📜 All Functions

```python
help(TextCleaner)
# or
dir(TextCleaner)
```

---

## 👨‍💻 Check Author & Metadata

```python
import importlib.metadata
print(importlib.metadata.metadata("justcleanme"))
```

Expected Output:

```
Name: justcleanme
Version: 0.1.0
Author: Rituraj Pandey
...
```

---

---

<!-- ## 📄 License

MIT License -->

---

## 🙋‍♂️ Author

**Rituraj Pandey**  

## 🤝 Contributions

Feel free to raise an issue or submit a pull request to improve this package!
