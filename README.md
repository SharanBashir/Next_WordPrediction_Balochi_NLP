# Balochi Next-Word Prediction using N-Gram Models

This project focuses on building a statistical language model for the Balochi language using N-gram models. It is capable of performing next-word prediction and analyzing the frequency of common N-grams (bigrams, trigrams, quadgrams) from a given Balochi corpus.

---

## 📂 Files in the Repository

* `balochi.txt`: The cleaned Balochi language corpus.
* `next_word_prediction.py`: Python script for building the N-gram model and performing prediction.
* `Balochi_NextWordPrediction.pkl`: Trained Lidstone N-gram model saved using dill.
* `README.md`: Description and documentation of the project.

---

## 🚀 Features

* Tokenization and N-gram generation (up to 4-grams)
* Text cleaning and padding
* Model training using Lidstone/Laplace/Kneser-Ney smoothing
* Perplexity evaluation on test set
* Most frequent bigrams, trigrams, and quadgrams
* Visualization using Plotly
* Model serialization with `dill`

---

## 🔍 How to Use

### Clone the Repo:

```bash
git clone https://github.com/SharanBashir/Next_WordPrediction_Balochi_NLP.git
cd Next_WordPrediction_Balochi_NLP
python next_word_prediction.py
```

### Run the Script:

```bash
python next_word_prediction.py
```

### Predict Next Words:

After training, enter any word when prompted to see top next-word predictions:

```python
input_text = (input('Enter a word: ')).split()
sorted(model.counts[input_text].most_common(3))
```

---

## 🌎 Dataset

The dataset used is a manually cleaned Balochi text corpus, with sentences separated by the "یے" punctuation mark.

---

## 🔧 Libraries Used

* `nltk` (language modeling)
* `pandas`, `numpy` (data handling)
* `plotly.express` (data visualization)
* `dill` (model saving)
* `collections.Counter`, `itertools.chain` (n-gram counting)

---

## 🏆 Results

* Trained model vocabulary: \~10,000 tokens
* Perplexity evaluated on test data
* Top 10 bigrams/trigrams/quadgrams visualized using interactive bar charts

---

## 📅 Author

Sharan Bashir
Final Year PG Research Project, Balochi Language Processing

---

## 👁️ License

This project is licensed under the MIT License. See the LICENSE file for details.
