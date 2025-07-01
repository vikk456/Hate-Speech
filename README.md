# 🧠 Hate Speech Detection using Machine Learning

This project aims to classify tweets into categories such as hate speech, offensive language, or neither using machine learning techniques. The pipeline involves data cleaning, feature extraction using `CountVectorizer`, and training models like **Bernoulli Naive Bayes** and **Logistic Regression**.

---

## 📂 Dataset

The dataset used is a CSV file (`train.csv`) containing:

- `tweet`: The tweet text
- `class`: Label
  - `0` = Hate Speech
  - `1` = Offensive Language
  - `2` = Neither

---

## ⚙️ Tools & Technologies

- Python
- Pandas & NumPy
- Scikit-learn
- CountVectorizer
- Logistic Regression
- Bernoulli Naive Bayes
- Regex for text preprocessing

---

## 🧼 Text Preprocessing

- Converted text to lowercase
- Removed URLs, punctuation, and extra whitespace using regex
- Removed English stopwords with `CountVectorizer(stop_words='english')`

---

## 🧪 Models Trained

| Model                  | Accuracy | Notes                           |
|-----------------------|----------|----------------------------------|
| Bernoulli Naive Bayes | ~85%     | Fast, good baseline              |
| Logistic Regression   | ~86–88%  | Balanced class weights improved performance |

---

## 📈 Evaluation

Model performance was evaluated using:
- **Accuracy**
- **Precision, Recall, F1-score**
- `classification_report` from `sklearn`

---

## 🚀 How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
